# セクションとページ構成を整理しよう

## **[section](https://developer.mozilla.org/ja/docs/Web/HTML/Element/section)**

<dl>
  <dt>意味・役割</dt>
  <dd>章・節・項など一般的なセクションを表す。<br>話題の階層をより明確にする役割を持つ。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>セクショニング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[article](https://developer.mozilla.org/ja/docs/Web/HTML/Element/article)**

<dl>
  <dt>意味・役割</dt>
  <dd>ブログやニュース記事などの独立したセクションを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>セクショニング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### section との使い分け

`section`は話題を構成する一部のイメージで、`article`はブログ等に投稿した場合、それだけで１つのコンテンツとして成り立つ内容のイメージ

## **[aside](https://developer.mozilla.org/ja/docs/Web/HTML/Element/aside)**

<dl>
  <dt>意味・役割</dt>
  <dd>メインコンテンツから切り離すことが可能な補足的なセクションを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>セクショニング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[nav](https://developer.mozilla.org/ja/docs/Web/HTML/Element/nav)**

<dl>
  <dt>意味・役割</dt>
  <dd>主要なナビゲーションを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>セクショニング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[address](https://developer.mozilla.org/ja/docs/Web/HTML/Element/address)**

<dl>
  <dt>意味・役割</dt>
  <dd>連絡先情報を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ<br>ただし、子孫にヘディング・コンテンツ, セクショニング・コンテンツ, header, footer, address要素は配置不可</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[header](https://developer.mozilla.org/ja/docs/Web/HTML/Element/header)**

<dl>
  <dt>意味・役割</dt>
  <dd>ヘッダーを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ<br>ただし、子孫にheader要素, footer要素は配置不可</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[footer](https://developer.mozilla.org/ja/docs/Web/HTML/Element/footer)**

<dl>
  <dt>意味・役割</dt>
  <dd>フッターを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ<br>ただし、子孫にheader要素, footer要素は配置不可</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[main](https://developer.mozilla.org/ja/docs/Web/HTML/Element/main)**

<dl>
  <dt>意味・役割</dt>
  <dd>メインコンテンツを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[div](https://developer.mozilla.org/ja/docs/Web/HTML/Element/div)**

<dl>
  <dt>意味・役割</dt>
  <dd>特に役割を持たない汎用的なブロックレベル。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ<br>dl要素の子要素の場合 ・・・ 1つ以上のdt要素とそれに続くdd要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[span](https://developer.mozilla.org/ja/docs/Web/HTML/Element/span)**

<dl>
  <dt>意味・役割</dt>
  <dd>特に役割を持たない汎用的なインラインレベル。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## アウトラインを意識する

html では話題の階層構造(アウトライン)を意識することが重要で`h1~h6`を使うことで生成されます。`hn`要素は必ず 1→6 で順に使用するようにする。
https://validator.w3.org/nu/ から確認可能
