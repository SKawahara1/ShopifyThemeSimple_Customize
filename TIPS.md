---
marp: true

---
<!-- 
theme: default
size: 16:9
paginate: true
style: |
  section {
    background-color: #FFFFFF;
  }
-->

# Google Fonts (Noto Sans JP)を使用する方法
参照: <https://note.com/gooddoctor/n/nce84b2ef484d>

参照リンクを見ればだいたいわかるはず、一応詳細を以下に記述

**layout/theme.liquid**の<head>タグ内にFontリンクを貼る

**assets/theme.scss.liquid** のプロパティ

- \$font-stack-header
- \$font-stack-body
- \$font-stack-cart-notification

でフォント値を**Noto Sans JP**と**sans-serif**にする
sans-serifのところ表示不可を回避するためのセーフフォントであれば何でも良い

---
# スライドバーの幅を伸ばす
CSSのGrid Layoutを使ってページ幅を分割し、レイアウトしている
この比率を変えてやれば幅を伸ばせる

**theme.scss.liquid**の1292行目～でクラスが定義されてる

```scss
  .#{$grid-breakpoint-type}one-third { width: percentage(1 / 3); }
  .#{$grid-breakpoint-type}two-thirds { width: percentage(2 / 3); }
```

**one-third**で3分割の1、**one-thirds**で3分割の2つ分という感じで
ページ幅からの分割数と比率を決めている

liquidファイルのクラス名これを入れればレイアウトできる

---

サイドバー幅を変更する場合、**layout/theme.liquid**, **sections/sidebar.liquid**
の2つのリキッドファイルにまたがって設定されているのを変更する

##### layout/theme.liquid: 66line~

```html
  <main class="main-content grid__item medium-up--four-fifths" id="MainContent" role="main">
```

&darr;

```html
  <main class="main-content grid__item medium-up--three-quarters" id="MainContent" role="main">
```

#### sections/sidebar.liquid: 2line~

```html
 <nav class="grid__item small--text-center medium-up--one-fifth" role="navigation">
```

&darr;

```html
 <nav class="grid__item small--text-center medium-up--one-quarter" role="navigation">
  ```

---

サイドバーが1/5,メインコンテンツが4/5のところを1/4, 3/4に変更することで、
ページ幅に占めるサイドバーの比率を上げている

### 注意
one-quarterのように左側の数字が1だと右は**quarter**と単数形だが
three-quartersのように左側が複数だと**quarters**と複数形になる
間違えやすいので注意

---

# リンクにマウスが乗った時に色を変える

### assets/theme.scss.liquid: 573line~

```css
 a:hover {
    background-color: rgb(162, 171, 255);
    outline: 0;
}
```

aタグ（リンクのセレクタ）:hoverでマウスが乗った時の設定ができる

---

# 背景色をグラデーションにする
linear-gradientで設定できる
ここでは3色でグラデーションを表している

### assets/theme.scss.liquid: 1503line~

```css
  body,
    html {
      /* background-color: $color-body; */
      background:
      linear-gradient(rgba(200,227,255,0.2),
                      rgba(246,250,255,0.2) 60%,
                      rgba(255,255,255,0.2));
    }
```

---

# ログインしたとき名前でなく姓が出るようにする

該当箇所のfirst_nameをlast_nameに変更

##### locales/ja.json: 263line~

```json
   "customer": {
      "account": "アカウント",
      "logged_in_as_html": "{{ last_name }}としてログインしました",
```

##### sections/header.liquid

```html
  {% if customer.last_name != blank %}
      {% capture last_name %}<a href="{{ routes.account_url }}">{{ customer.last_name }}</a>{% endcapture %}
      {{ 'layout.customer.logged_in_as_html' | t: last_name: last_name }}
```

---

# 住所入力フォームの順番を入れ替える
「新しい住所を追加する」場合、liquidファイルの該当箇所は
#### templates/customers/addresses.liquid: 19~92line

```html
<div id="AddressNewForm" class="form-address form-vertical hide">
  {% form 'customer_address', customer.new_address %}
    <div class="grid"></div>
    <div class="grid"></div>
    .
    .
</div>
```

というコード構成になっている
<class="grid">内の<class="grid-item">にフォーム項目が入っているので
その順番を入れ替える

---
もともとは英語圏向けの並びになっているので、日本向けに
[姓] [名] [郵便番号] [国] [都道府県] [市町村] [番地] [建物/部屋番号] [会社名] [電話番号]
と並び替える

仕様では「国」は日本で確定のため削除ということだが、「国」フォームをコードから消すとエラーになるので
#### templates/customers/addresses.liquid

 ```html
  <div class="grid__item hide">
    <label for="AddressCountryNew">{{ 'customer.addresses.country' | t }}</label>
```

のように親要素のクラス名に hide を入れ、見た目上消すことで対処する

---
「国」フォームをコードから消すとエラーになる理由はShopifyの住所テンプレートの仕様から外れるからだと思われる

参照：[Shopify Developers](https://shopify.dev/docs/themes/files/customers-addresses-liquid)

ユーザーのフォーム入力が空でも送信できるが、
このリンク先の表にあるform typeとname attributeが一致しないと送信できない

郵便番号入力フォームを2つに分割できないのもこれが原因

---
# フォームの特定項目にフォーカスする
#### assets/theme.js.liquid: 253-267line

```javascript
  const focusMethod = (id)=> {
    document.getElementById(id).focus();
  }
  // Toggle new/edit address forms
  $('.address-new-toggle').on('click', function() {
    $newAddressForm.toggleClass('hide');
    focusMethod('AddressZipNew');
  });
```

document.getElementById().focus()でフォームの項目にフォーカスできる
引数idにはフォーカス先のidを入れる
.address-new-toggleクラスの住所作成ボタンをクリックした時に実行される

---
# フォームの項目を事前に入力し、変更不可にする

formのinputタグで設定する
#### templates/customers/addresses.liquid: 27line

```html
 <input type="text"
        id="AddressLastNameNew" name="address[last_name]"
        value="{{ customer.last_name }}"
        autocapitalize="words"
        readonly>
```

valueでデフォルト値を設定できるので、顧客情報データから{{ customer.last_name }}のようにして持ってくる
readonly属性を入れると変更不可になる

---
# 郵便番号から住所を自動入力

ajaxzip3ライブラリを使って自動入力する
参照：<https://github.com/ajaxzip3/ajaxzip3.github.io>
<https://haniwaman.com/ajaxzip3/>

#### templates/customers/address.liquid 40-42line

```html
<label for="AddressZipNew">{{ 'customer.addresses.zip' | t }}</label>
<script src="https://ajaxzip3.github.io/ajaxzip3.js" charset="UTF-8"></script>

 <input type="text"
        ...
        onKeyUp="AjaxZip3.zip2addr(this,'','address[province]','address[city]');">
```

onKeyUp(キーボードを離した時)、郵便番号が該当すれば都道府県(province)と市町村(city)に自動入力される
