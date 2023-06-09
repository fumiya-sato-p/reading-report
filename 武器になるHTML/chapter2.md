# テキストやリストをマークアップしよう

## **[[h1~h6]](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements)**

<dl>
  <dt>意味・役割</dt>
  <dd>headingの意味で、見出しを表す。<br>話題の階層を意識するために使用する。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ, ヘディング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[p](https://developer.mozilla.org/ja/docs/Web/HTML/Element/p)**

<dl>
  <dt>意味・役割</dt>
  <dd>paragraphの意味で、段落を表す。<br>話題の階層を意識するために使用する。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[br](https://developer.mozilla.org/ja/docs/Web/HTML/Element/br)**

<dl>
  <dt>意味・役割</dt>
  <dd>line breakの意味で、改行を表す。終了タグが必要ない。</dd>
</dl>

## **[em](https://developer.mozilla.org/ja/docs/Web/HTML/Element/em)**

<dl>
  <dt>意味・役割</dt>
  <dd>emphasisの意味で、強調を表す。<br>複数重ねて使用することで強度を変えることができる。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ, フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[strong](https://developer.mozilla.org/ja/docs/Web/HTML/Element/strong)**

<dl>
  <dt>意味・役割</dt>
    <dd>重要性や深刻さ、緊急性を表す。<br>複数重ねて使用することで強度を変えることができる。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ, フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[small](https://developer.mozilla.org/ja/docs/Web/HTML/Element/small)**

<dl>
  <dt>意味・役割</dt>
  <dd>著作権表記や警告、法的制限、免責事項のようなサイドコメントを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ, フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[time](https://developer.mozilla.org/ja/docs/Web/HTML/Element/time)**

<dl>
  <dt>意味・役割</dt>
  <dd>日付や時刻、タイムゾーンオフセットなどを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ, フレージング・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>datetime属性を指定している場合はフレージング・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性<br>datetime属性・・・コンピューターが理解できる日時</dd>
</dl>

コンピューターが理解できるフォーマット
| 表示項目 | 例 | 説明 |
|:---:|---|---|
| 年 | 2022 | 4 桁の西暦 |
| 年月 | 2022-01 | 4 桁の西暦-2 桁の月 |
| 年月日 | 2022-01-01 | 4 桁の西暦-2 桁の月-2 桁の日 |
| 月日 | 01-01 | 2 桁の月-2 桁の日 |
| 時分 | 01:01 | 2 桁の時:2 桁の分 |
| 時分秒 | 01:01:01 | 2 桁の時:2 桁の分:2 桁の秒 |
| 年月日時分秒 | 2022-01-01 01:01:01 | 4 桁の西暦-2 桁の月-2 桁の日 2 桁の時:2 桁の分:2 桁の秒 |

```html
datetimeなし: <time>2022-01-01 01:01:01</time>

datetimeあり: <time datetime="2022-01">2022年1月</time>
```

## **[li](https://developer.mozilla.org/ja/docs/Web/HTML/Element/li)**

<dl>
  <dt>意味・役割</dt>
  <dd>list itemの意味で、リスト項目を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性<br>[親がol] value属性・・・リストの番号を指定</dd>
</dl>

## **[ul](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ul)**

<dl>
  <dt>意味・役割</dt>
  <dd>unorderd listの意味で、順不同リストを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>0個以上のli, スクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[ol](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ol)**

<dl>
  <dt>意味・役割</dt>
  <dd>orderd listの意味で、番号順リストを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>0個以上のli, スクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    reverse属性 --- リストの番号を逆順にする<br>
    start属性 --- 開始番号を指定する<br>
    type属性 --- リストの番号の種類を指定する
  </dd>
</dl>

type 属性で指定できる種類
| 値 | 説明 |
| :------------: | -------------- |
| 1 | 10 進数の数字 |
| a | 小文字のラテンアルファベット |
| A | 大文字のラテンアルファベット |
| i | 小文字のローマ数字 |
| I | 大文字のローマ数字 |

## **[dl](https://developer.mozilla.org/ja/docs/Web/HTML/Element/dl)**

<dl>
  <dt>意味・役割</dt>
  <dd>description listの意味で、説明リストを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>0個以上のdd・dtの組み合わせ, 1つ以上のdiv要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[dt](https://developer.mozilla.org/ja/docs/Web/HTML/Element/dt)**

<dl>
  <dt>意味・役割</dt>
  <dd>description listのtermの意味で、説明する項目名や用語部分を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ（子孫にheader, footer, セクショニング, ヘディングは不可）</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[dd](https://developer.mozilla.org/ja/docs/Web/HTML/Element/dd)**

<dl>
  <dt>意味・役割</dt>
  <dd>description listのdescription, definitionの意味で、説明リストの説明, 定義, 値を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## 特殊な記述が必要な文字

| 表示される文字 | 名前付き文字参照 | 数値文字参照 |
| :------------: | :--------------: | :----------: |
|       <        |      `&lt;`      |    `&#60`    |
|       >        |      `&gt;`      |    `&#62`    |
|       &        |     `&amp;`      |    `&#38`    |
|       "        |     `&quot;`     |   `&#34;`    |
|       ©        |     `&copy;`     |   `&#169;`   |
|       ®        |     `&reg;`      |   `&#174;`   |
|       ™        |    `&trade;`     |  `&#8482;`   |

名前付き文字参照の方が英単語をベースにしているため、よく使われる。  
その他の文字は[こちら](https://html.spec.whatwg.org/multipage/named-characters.html)

## その他
