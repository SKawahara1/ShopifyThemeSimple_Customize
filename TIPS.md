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
参照: https://note.com/gooddoctor/n/nce84b2ef484d

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

##### layout/theme.liquid
```html
66  <main class="main-content grid__item medium-up--four-fifths" id="MainContent" role="main">
```
&darr;
```html
66  <main class="main-content grid__item medium-up--three-quarters" id="MainContent" role="main">
```

**sections/sidebar.liquid**
```html
2  <nav class="grid__item small--text-center medium-up--one-fifth" role="navigation">
```
&darr;
```html
2  <nav class="grid__item small--text-center medium-up--one-quarter" role="navigation">
  ```

---

サイドバーが1/5,メインコンテンツが4/5のところを1/4, 3/4に変更することで、
ページ幅に占めるサイドバーの比率を上げている

### 注意: 
one-quarterのように左側の数字が1だと右は**quarter**と単数形だが
three-quartersのように左側が複数形だと**quarters**と複数形になる
間違えやすいので注意

---

# リンクにマウスが乗った時に色を変える

### assets/theme.scss.liquid
```css
573 a:hover {
      background-color: rgb(162, 171, 255);
      outline: 0;
}
```

<a>タグ（リンクのセレクタ）:hoverでマウスが乗った時の設定ができる

---

# 背景色をグラデーションにする
linear-gradientで設定できる
ここでは3色でグラデーションを表している

### assets/theme.scss.liquid
```css
1503    body,
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