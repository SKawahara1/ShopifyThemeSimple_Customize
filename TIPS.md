<!-- TOC -->

- [Google Fonts Noto Sans JPを使用する方法](#google-fonts-noto-sans-jp%E3%82%92%E4%BD%BF%E7%94%A8%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95)
- [スライドバーの幅を伸ばす](#%E3%82%B9%E3%83%A9%E3%82%A4%E3%83%89%E3%83%90%E3%83%BC%E3%81%AE%E5%B9%85%E3%82%92%E4%BC%B8%E3%81%B0%E3%81%99)
- [リンクにマウスが乗った時に色を変える](#%E3%83%AA%E3%83%B3%E3%82%AF%E3%81%AB%E3%83%9E%E3%82%A6%E3%82%B9%E3%81%8C%E4%B9%97%E3%81%A3%E3%81%9F%E6%99%82%E3%81%AB%E8%89%B2%E3%82%92%E5%A4%89%E3%81%88%E3%82%8B)
- [背景色をグラデーションにする](#%E8%83%8C%E6%99%AF%E8%89%B2%E3%82%92%E3%82%B0%E3%83%A9%E3%83%87%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E3%81%AB%E3%81%99%E3%82%8B)
- [ログインしたとき名前でなく姓が出るようにする](#%E3%83%AD%E3%82%B0%E3%82%A4%E3%83%B3%E3%81%97%E3%81%9F%E3%81%A8%E3%81%8D%E5%90%8D%E5%89%8D%E3%81%A7%E3%81%AA%E3%81%8F%E5%A7%93%E3%81%8C%E5%87%BA%E3%82%8B%E3%82%88%E3%81%86%E3%81%AB%E3%81%99%E3%82%8B)
- [住所入力フォームの順番新規作成時を入れ替える](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E3%81%AE%E9%A0%86%E7%95%AA%E6%96%B0%E8%A6%8F%E4%BD%9C%E6%88%90%E6%99%82%E3%82%92%E5%85%A5%E3%82%8C%E6%9B%BF%E3%81%88%E3%82%8B)
  - [住所入力フォーム新規作成時の順番を入れ替える-　コピー用コード](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E6%96%B0%E8%A6%8F%E4%BD%9C%E6%88%90%E6%99%82%E3%81%AE%E9%A0%86%E7%95%AA%E3%82%92%E5%85%A5%E3%82%8C%E6%9B%BF%E3%81%88%E3%82%8B-%E3%80%80%E3%82%B3%E3%83%94%E3%83%BC%E7%94%A8%E3%82%B3%E3%83%BC%E3%83%89)
  - [住所入力フォーム編集時の順番を入れ替える-　コピー用コード](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E7%B7%A8%E9%9B%86%E6%99%82%E3%81%AE%E9%A0%86%E7%95%AA%E3%82%92%E5%85%A5%E3%82%8C%E6%9B%BF%E3%81%88%E3%82%8B-%E3%80%80%E3%82%B3%E3%83%94%E3%83%BC%E7%94%A8%E3%82%B3%E3%83%BC%E3%83%89)
- [フォームの特定項目にフォーカスする](#%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E3%81%AE%E7%89%B9%E5%AE%9A%E9%A0%85%E7%9B%AE%E3%81%AB%E3%83%95%E3%82%A9%E3%83%BC%E3%82%AB%E3%82%B9%E3%81%99%E3%82%8B)
- [フォームの項目を事前に入力し、変更不可にする](#%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E3%81%AE%E9%A0%85%E7%9B%AE%E3%82%92%E4%BA%8B%E5%89%8D%E3%81%AB%E5%85%A5%E5%8A%9B%E3%81%97%E5%A4%89%E6%9B%B4%E4%B8%8D%E5%8F%AF%E3%81%AB%E3%81%99%E3%82%8B)
- [郵便番号から住所を自動入力する](#%E9%83%B5%E4%BE%BF%E7%95%AA%E5%8F%B7%E3%81%8B%E3%82%89%E4%BD%8F%E6%89%80%E3%82%92%E8%87%AA%E5%8B%95%E5%85%A5%E5%8A%9B%E3%81%99%E3%82%8B)
- [入力フォームのスタイルを変更する](#%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E3%81%AE%E3%82%B9%E3%82%BF%E3%82%A4%E3%83%AB%E3%82%92%E5%A4%89%E6%9B%B4%E3%81%99%E3%82%8B)
- [住所入力フォームテキスト入力タイプにグレー文字の初期値を設定する](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E3%83%86%E3%82%AD%E3%82%B9%E3%83%88%E5%85%A5%E5%8A%9B%E3%82%BF%E3%82%A4%E3%83%97%E3%81%AB%E3%82%B0%E3%83%AC%E3%83%BC%E6%96%87%E5%AD%97%E3%81%AE%E5%88%9D%E6%9C%9F%E5%80%A4%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%99%E3%82%8B)
- [住所入力フォーム選択タイプに初期値を設定する](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A9%E3%83%BC%E3%83%A0%E9%81%B8%E6%8A%9E%E3%82%BF%E3%82%A4%E3%83%97%E3%81%AB%E5%88%9D%E6%9C%9F%E5%80%A4%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%99%E3%82%8B)
- [住所入力フィールドのラベルを変更する](#%E4%BD%8F%E6%89%80%E5%85%A5%E5%8A%9B%E3%83%95%E3%82%A3%E3%83%BC%E3%83%AB%E3%83%89%E3%81%AE%E3%83%A9%E3%83%99%E3%83%AB%E3%82%92%E5%A4%89%E6%9B%B4%E3%81%99%E3%82%8B)

<!-- /TOC -->

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

サイドバーが1/5,メインコンテンツが4/5のところを1/4, 3/4に変更することで、
ページ幅に占めるサイドバーの比率を上げている

### 注意

one-quarterのように左側の数字が1だと右は**quarter**と単数形だが
three-quartersのように左側が複数だと**quarters**と複数形になる
間違えやすいので注意

# リンクにマウスが乗った時に色を変える

### assets/theme.scss.liquid: 573line~

```css
 a:hover {
    background-color: rgb(162, 171, 255);
    outline: 0;
}
```

aタグ（リンクのセレクタ）:hoverでマウスが乗った時の設定ができる

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

# 住所入力フォームの順番(新規作成時)を入れ替える

「新しい住所を追加する」場合、liquidファイルの該当箇所は

#### templates/customers/addresses.liquid: 19~89line

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

もともとは英語圏向けの並びになっているので、日本向けに
[姓] [名] [郵便番号] [国] [都道府県] [市町村] [番地] [建物/部屋番号] [電話番号] [会社名]
と並び替える

仕様では「国」は日本で確定のため削除ということだが、「国」フォームをコードから消すとエラーになるので

#### templates/customers/addresses.liquid

 ```html
  <div class="grid__item hide">
    <label for="AddressCountryNew">{{ 'customer.addresses.country' | t }}</label>
```

のように親要素のクラス名に hide を入れ、見た目上消すことで対処する

「国」フォームをコードから消すとエラーになる理由はShopifyの住所テンプレートの仕様から外れるからだと思われる

参照：[Shopify Developers - customers/addresses.liquid](https://shopify.dev/docs/themes/files/customers-addresses-liquid)

ユーザーのフォーム入力が空でも送信できるが、
このリンク先の表にあるform typeとname attributeが一致しないと送信できない

郵便番号入力フォームを2つに分割できないのもこれが原因

## 住所入力フォーム(新規作成時)の順番を入れ替える-　コピー用コード

templates/customers/addresses.liquidの19～89行目を消し、下のコードをコピーして挿入すれば日本用の項目順になる

```html
<div id="AddressNewForm" class="form-address form-vertical hide">

  {% form 'customer_address', customer.new_address %}

    <div class="grid">

      <div class="grid__item">
        <label for="AddressLastNameNew">{{ 'customer.addresses.last_name' | t }}</label>
        <input type="text" id="AddressLastNameNew" name="address[last_name]" value="{{ customer.last_name }}" autocapitalize="words" readonly>
      </div>

      <div class="grid__item">
        <label for="AddressFirstNameNew">{{ 'customer.addresses.first_name' | t }}</label>
        <input type="text" id="AddressFirstNameNew" name="address[first_name]" value="{{ customer.first_name }}" autocapitalize="words" readonly>
      </div>

    </div>

    <div class="grid">

      <div class="grid__item">
        <label for="AddressZipNew">{{ 'customer.addresses.zip' | t }}</label>
        <script src="https://ajaxzip3.github.io/ajaxzip3.js" charset="UTF-8"></script>
        <input type="text" id="AddressZipNew" name="address[zip]" value="{{ form.zip }}" autocapitalize="characters" maxlength="8" onKeyUp="AjaxZip3.zip2addr(this,'','address[province]','address[city]');">
      </div>
      <div class="grid__item hide">
        <label for="AddressCountryNew">{{ 'customer.addresses.country' | t }}</label>
        <select id="AddressCountryNew" name="address[country]" data-default="{{ form.country }}">{{ all_country_option_tags }}</select>
        {% comment %} <input type="text" id="AddressCountryNew" name="address[country]" value="{{ form.country }}" autocapitalize="words"> {% endcomment %}
      </div>

      <div class="grid__item" id="AddressProvinceContainerNew">
        <label for="AddressProvinceNew">{{ 'customer.addresses.province' | t }}</label>
        <select id="AddressProvinceNew" name="address[province]" data-default="{{ form.province }}"></select>
        {% comment %} <input type="text" id="AddressProvinceNew" name="address[province]" value="{{ form.province }}" autocapitalize="words"> {% endcomment %}
      </div>
      <div class="grid__item">
        <label for="AddressCityNew">{{ 'customer.addresses.city' | t }}</label>
        <input type="text" id="AddressCityNew" name="address[city]" value="{{ form.city }}" autocapitalize="words">
      </div>

      <div class="grid__item">

        <label for="AddressAddress1New">{{ 'customer.addresses.address1' | t }}</label>
        <input type="text" id="AddressAddress1New" name="address[address1]" value="{{ form.address1 }}" autocapitalize="words">

        <label for="AddressAddress2New">{{ 'customer.addresses.address2' | t }}</label>
        <input type="text" id="AddressAddress2New" name="address[address2]" value="{{ form.address2 }}" autocapitalize="words">
      </div>

    </div>

    <div class="grid">
      <div class="grid__item">
        <label for="AddressPhoneNew">{{ 'customer.addresses.phone' | t }}</label>
        <input type="tel" id="AddressPhoneNew" name="address[phone]" value="{{ form.phone }}">

        <label for="AddressCompanyNew">{{ 'customer.addresses.company' | t }}</label>
        <input type="text" id="AddressCompanyNew" name="address[company]" value="{{ form.company }}" autocapitalize="words">
      </div>

    </div>

    <p>
      {{ form.set_as_default_checkbox }}
      <label for="address_default_address_new">{{ 'customer.addresses.set_default' | t }}</label>
    </p>

    <p><input type="submit" class="btn" value="{{ 'customer.addresses.add' | t }}"></p>
    <p><button type="button" class="btn--link address-new-toggle">{{ 'customer.addresses.cancel' | t }}</button></p>

  {% endform %}
</div>

```

## 住所入力フォーム(編集時)の順番を入れ替える-　コピー用コード

#### templates/customers/addresses.liquid: 113-17line

```html
  <div id="EditAddress_{{ address.id }}" class="hide form-vertical">
    {% form 'customer_address', address %}
    ...(略)
    {% endform %}
  </div>
```

の部分を消し、以下のコピーを挿入する

```html
  <div id="EditAddress_{{ address.id }}" class="hide form-vertical">
    {% form 'customer_address', address %}

      <h3 class="h4">{{ 'customer.addresses.edit_address' | t }}</h3>

    <div class="grid">

      <div class="grid__item">
        <label for="AddressLastName_{{ form.id }}">{{ 'customer.addresses.last_name' | t }}</label>
        <input type="text" id="AddressLastName_{{ form.id }}" name="address[last_name]" value="{{ form.last_name }}" autocapitalize="words">
      </div>

      <div class="grid__item">
        <label for="AddressFirstName_{{ form.id }}">{{ 'customer.addresses.first_name' | t }}</label>
        <input type="text" id="AddressFirstName_{{ form.id }}" name="address[first_name]" value="{{ form.first_name }}" autocapitalize="words">
      </div>

    </div>

    <label for="AddressZip_{{ form.id }}">{{ 'customer.addresses.zip' | t }}</label>
    <input type="text" id="AddressZip_{{ form.id }}" name="address[zip]" value="{{ form.zip }}" autocapitalize="characters" maxlength="8" onKeyUp="AjaxZip3.zip2addr(this,'','address[province]','address[city]');">
  
    <div class = "hide">
      <label for="AddressCountry_{{ form.id }}">{{ 'customer.addresses.country' | t }}</label>
      <select id="AddressCountry_{{ form.id }}" class="address-country-option" data-form-id="{{ form.id }}" name="address[country]" data-default="{{ form.country }}">{{ all_country_option_tags }}</select>
    </div>
  
    <div id="AddressProvinceContainer_{{ form.id }}">
      <label for="AddressProvince_{{ form.id }}">{{ 'customer.addresses.province' | t }}</label>
      <select id="AddressProvince_{{ form.id }}" name="address[province]" data-default="{{ form.province }}"></select>
    </div>

    <label for="AddressCity_{{ form.id }}">{{ 'customer.addresses.city' | t }}</label>
    <input type="text" id="AddressCity_{{ form.id }}" name="address[city]" value="{{ form.city }}" autocapitalize="words">

    <label for="AddressAddress1_{{ form.id }}">{{ 'customer.addresses.address1' | t }}</label>
    <input type="text" id="AddressAddress1_{{ form.id }}" name="address[address1]" value="{{ form.address1 }}" autocapitalize="words">

    <label for="AddressAddress2_{{ form.id }}">{{ 'customer.addresses.address2' | t }}</label>
    <input type="text" id="AddressAddress2_{{ form.id }}" name="address[address2]" value="{{ form.address2 }}" autocapitalize="words">
  

    <div class="grid">
      <div class="grid__item">
        <label for="AddressPhone_{{ form.id }}">{{ 'customer.addresses.phone' | t }}</label>
        <input type="tel" id="AddressPhone_{{ form.id }}" name="address[phone]" value="{{ form.phone }}">

        <label for="AddressCompany_{{ form.id }}">{{ 'customer.addresses.company' | t }}</label>
        <input type="text" id="AddressCompany_{{ form.id }}" name="address[company]" value="{{ form.company }}" autocapitalize="words">
      </div>

    </div>
      <p>
        {{ form.set_as_default_checkbox }}
        <label for="address_default_address_{{ form.id }}">{{ 'customer.addresses.set_default' | t }}</label>
      </p>

      <p><input type="submit" class="btn" value="{{ 'customer.addresses.update' | t }}"></p>
      <p><button type="button" class="btn--link address-edit-toggle" data-form-id="{{ form.id }}">{{ 'customer.addresses.cancel' | t }}</button></p>

    {% endform %}
  </div>
```

# フォームの特定項目にフォーカスする

#### assets/theme.js.liquid: 254-257ine

```javascript
  // Toggle new/edit address forms
  $('.address-new-toggle').on('click', function() {
    $newAddressForm.toggleClass('hide');
  });
```

theme.js.liquidの254-257行目の上記コードを以下のように変更する

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

`focusMethod('AddressZipNew');`の`'AddressZipNew'`を変更することでフォーカス先を変えられる<br>

例):

- `'AddressZipNew'` → `'AddressLastNameNew'`　で「姓」フォーム
- `'AddressZipNew'` → `'AddressFirstNameNew'`　で「名前」フォーム

document.getElementById().focus()でフォームの項目にフォーカスできる
`focusMethod(id)`の引数idはフォーカス先のidを入れる
住所作成ボタン(.address-new-toggle)をクリックした時に実行される

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

# 郵便番号から住所を自動入力する

ajaxzip3ライブラリを使って自動入力する
参照：<https://github.com/ajaxzip3/ajaxzip3.github.io>
-<https://haniwaman.com/ajaxzip3/>

#### templates/customers/address.liquid 40-42line

```html
<label for="AddressZipNew">{{ 'customer.addresses.zip' | t }}</label>
<script src="https://ajaxzip3.github.io/ajaxzip3.js" charset="UTF-8"></script>

 <input type="text"
        ...
        onKeyUp="AjaxZip3.zip2addr(this,'','address[province]','address[city]');">
```

onKeyUp(キーボードを離した時)、郵便番号が該当すれば都道府県(province)と市町村(city)に自動入力される
郵便番号は8桁まで入力可能で、ハイフンあり/なしのどちらでも自動入力される

# 入力フォームのスタイルを変更する

入力フォームのセル色はテーマのカスタマイズから変更できる

![a](https://imgur.com/2C90VMy.png)
テーマ設定→色

&darr;

![a](https://i.imgur.com/PoTqnwH.png)
フォームフィールドの背景

**フォームの枠線**は、

#### assets/theme.scss.liquid 2639-2650line

```css
.form-vertical {
  input,
  select,
  textarea {
    display: block;
    margin-bottom: $padding-form;
    min-width: 300px;

    @include media-query($small) {
      width: 100%;
    }
  }
```

`min-width:300px;`の下の行に`border: 1px solid #000;`を挿入すれば枠線が表示される
枠線のスタイルを変更したいときは[こちら](https://techacademy.jp/magazine/8626)を参照

# 住所入力フォーム(テキスト入力タイプ)にグレー文字の初期値を設定する

htmlのinput要素にplaceholder属性を追加すると初期値を設定できる [こちらを参照](https://weback.net/htmlcss/1284/)
**注意:** placeholderで初期値を設定できるのはテキスト入力の項目のみで、都道府県項目のように選択タイプだと設定できない
選択タイプの設定方法は次に説明する

#### templates/customers/address.liquid 19-89line

```html
<div id="AddressNewForm" class="form-address form-vertical hide">

  {% form 'customer_address', customer.new_address %}
      ...(略)
  {% endform %}
</div>
```

の所を以下のコードに置き換えれば設定できる

```html
<div id="AddressNewForm" class="form-address form-vertical hide">

  {% form 'customer_address', customer.new_address %}

    <div class="grid">

      <div class="grid__item">
        <label for="AddressLastNameNew">{{ 'customer.addresses.last_name' | t }}</label>
        <input type="text" id="AddressLastNameNew" name="address[last_name]" value="{{ customer.last_name }}" autocapitalize="words" readonly>
      </div>

      <div class="grid__item">
        <label for="AddressFirstNameNew">{{ 'customer.addresses.first_name' | t }}</label>
        <input type="text" id="AddressFirstNameNew" name="address[first_name]" value="{{ customer.first_name }}" autocapitalize="words" readonly>
      </div>

    </div>

    <div class="grid">

      <div class="grid__item">
        <label for="AddressZipNew">{{ 'customer.addresses.zip' | t }}</label>
        <script src="https://ajaxzip3.github.io/ajaxzip3.js" charset="UTF-8"></script>
        <input type="text" id="AddressZipNew" name="address[zip]" value="{{ form.zip }}" autocapitalize="characters" maxlength="8" placeholder="128443"
        onKeyUp="AjaxZip3.zip2addr(this,'','address[province]','address[city]');">
      </div>
      <div class="grid__item hide">
        <label for="AddressCountryNew">{{ 'customer.addresses.country' | t }}</label>
        <select id="AddressCountryNew" name="address[country]" data-default="{{ form.country }}">{{ all_country_option_tags }}</select>
        {% comment %} <input type="text" id="AddressCountryNew" name="address[country]" value="{{ form.country }}" autocapitalize="words"> {% endcomment %}
      </div>

      <div class="grid__item" id="AddressProvinceContainerNew">
        <label for="AddressProvinceNew">{{ 'customer.addresses.province' | t }}</label>
        <select id="AddressProvinceNew" name="address[province]" data-default="{{ form.province }}"></select>
        {% comment %} <input type="text" id="AddressProvinceNew" name="address[province]" value="{{ form.province }}" autocapitalize="words"> {% endcomment %}
      </div>
      <div class="grid__item">
        <label for="AddressCityNew">{{ 'customer.addresses.city' | t }}</label>
        <input type="text" id="AddressCityNew" name="address[city]" value="{{ form.city }}" autocapitalize="words" placeholder="京都市伏見区竹田藁屋町">
      </div>

      <div class="grid__item">

        <label for="AddressAddress1New">{{ 'customer.addresses.address1' | t }}</label>
        <input type="text" id="AddressAddress1New" name="address[address1]" value="{{ form.address1 }}" autocapitalize="words" placeholder="50">

        <label for="AddressAddress2New">{{ 'customer.addresses.address2' | t }}</label>
        <input type="text" id="AddressAddress2New" name="address[address2]" value="{{ form.address2 }}" autocapitalize="words" placeholder="増田医科器械ビル 101">
      </div>

    </div>

    <div class="grid">
      <div class="grid__item">
        <label for="AddressPhoneNew">{{ 'customer.addresses.phone' | t }}</label>
        <input type="tel" id="AddressPhoneNew" name="address[phone]" value="{{ form.phone }}">

        <label for="AddressCompanyNew">{{ 'customer.addresses.company' | t }}</label>
        <input type="text" id="AddressCompanyNew" name="address[company]" value="{{ form.company }}" autocapitalize="words">
      </div>

    </div>

    <p>
      {{ form.set_as_default_checkbox }}
      <label for="address_default_address_new">{{ 'customer.addresses.set_default' | t }}</label>
    </p>

    <p><input type="submit" class="btn" value="{{ 'customer.addresses.add' | t }}"></p>
    <p><button type="button" class="btn--link address-new-toggle">{{ 'customer.addresses.cancel' | t }}</button></p>

  {% endform %}
</div>
```

# 住所入力フォーム(選択タイプ)に初期値を設定する

#### assets/theme.js.liquid231-240

```javascript
  // Initialize observers on address selectors, defined in shopify_common.js
  if (Shopify) {
    new Shopify.CountryProvinceSelector(
      'AddressCountryNew',
      'AddressProvinceNew',
      {
        hideElement: 'AddressProvinceContainerNew'
      }
    );
  }
```

の箇所を以下のコードに変更する

```javascript
  const selectInitialProvince = (provinceName) =>{
    const provinceOptions =  document.getElementById('AddressProvinceNew').options;
    const provinceArray = [].slice.call(provinceOptions);
    const indexNum = provinceArray.findIndex(option => option.value === provinceName);
    provinceOptions[indexNum].selected = true;
  }
  // Initialize observers on address selectors, defined in shopify_common.js
  if (Shopify) {
    new Shopify.CountryProvinceSelector(
      'AddressCountryNew',
      'AddressProvinceNew',
      {
        hideElement: 'AddressProvinceContainerNew'
      }
    );
    selectInitialProvince('Kyōto');
  }
```

`const provinceOptions =  document.getElementById('AddressProvinceNew').options;`
で都道府県の[select 要素に含まれる option 要素をすべて取得する](https://developer.mozilla.org/ja/docs/Web/API/HTMLSelectElement/options)

`const provinceArray = [].slice.call(provinceOptions);`
取得したoption要素は配列ではないので、[配列に変換する](https://lab.syncer.jp/Web/JavaScript/Snippet/53/)  

`const indexNum = provinceArray.findIndex(option => option.value === provinceName);`  
配列から引数`provinceName`の[index番号を取得する](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex)  

`provinceOptions[indexNum].selected = true;`  
取得したindex番号から初期値に設定したいoption要素を導き、[初期値として設定する](https://techacademy.jp/magazine/24290)  

`selectInitialProvince('Kyōto');`で引数に京都を設定し、実行する  
`Kyoto`ではなく`Kyōto`なことに注意  

# 住所入力フィールドのラベルを変更する

#### locales/ja.json 153-154line

```json
  "address1": "住所",
  "address2": "住所",
```

を

```json
  "address1": "地名\/番地",
  "address2": "建物名\/部屋番号",
```

に変更する  
`"地名\/番地",`の`\`はjsonファイルにおける[/(スラッシュ)文字のエスケープ処理](https://www.ipentec.com/document/json-character-escape)
