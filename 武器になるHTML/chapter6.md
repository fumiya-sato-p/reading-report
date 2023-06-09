# より良いページを作ろう

## **[meta](https://developer.mozilla.org/ja/docs/Web/HTML/Element/meta)**

<dl>
  <dt>意味・役割</dt>
  <dd>メタデータを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>メタデータ・コンテンツ<br>itemprop属性を持つ場合 ・・・ フロー・コンテンツ, セクショニング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    name ・・・ メタ情報の名前を表す<br>
    http-equiv ・・・ HTTPレスポンスヘッダーの情報を指定する<br>
    content ・・・ name属性またはhttp-equiv属性で指定した情報の種類に対する内容を指定する<br>
    charset ・・・ 文字エンコーディングを指定する<br>
    property ・・・ OGO等の情報の種類を指定する
  </dd>
</dl>

### name 属性

| 値          | 説明                           |
| ----------- | ------------------------------ |
| author      | ページの制作者                 |
| description | ページの紹介文                 |
| generator   | ページ制作に使用したソフト     |
| keywords    | ページのキーワード             |
| robots      | 検索エンジンのクローラーの制御 |

### property 属性

| 値             | 説明                         |
| -------------- | ---------------------------- |
| og:url         | ページの URL                 |
| og:title       | ページのタイトル             |
| og:description | ページの紹介文               |
| og:image       | ページのサムネイル画像の URL |
| og:type        | ページの種類                 |
| og:locale      | ページの言語                 |
| og:site_name   | サイト名                     |
| fb:app_id      | Facebook の App Id           |

他にも twitter 用など様々なプロパティがある

### 使い方

```html
<!-- 文字エンコーディングの指定 -->
<meta charset="UTF-8" />

<!-- IEで表示した際に最新の環境で表示する指定 -->
<meta http-equiv="X-UA-Compatible" content="IE=edge" />

<!-- 表示領域のレスポンシブ設定 -->
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

## **[link](https://developer.mozilla.org/ja/docs/Web/HTML/Element/link)**

<dl>
  <dt>意味・役割</dt>
  <dd>外部のリソースとリンクを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>メタデータ・コンテンツ<br>要素がbody内で許容されている場合 ・・・ フロー・コンテンツ, フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    href ・・・ リンク先を指定する<br>
  　rel ・・・ リソースとの関係を指定する<br>
    sizes ・・・ アイコンサイズを指定する<br>
    type ・・・ アイコン画像のファイル形式を指定する
  </dd>
</dl>

### rel 属性

| 値         | 説明                           |
| ---------- | ------------------------------ |
| canonical  | ページに対して正規化したい URL |
| icon       | アイコン                       |
| stylesheet | スタイルシート(CSS)            |
