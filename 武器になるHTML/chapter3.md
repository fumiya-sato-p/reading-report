# リンクやコンテンツを埋め込もう

## トランスペアレント

トランスペアレント(透明)がコンテンツ・モデルとして記載されている場合、その要素のコンテンツ・モデルは親要素のコンテンツ・モデルと同一になる  
トランスペアレントの由来は`ないものとみている = いないもの`から来ている

## **[a](https://developer.mozilla.org/ja/docs/Web/HTML/Element/a)**

<dl>
  <dt>意味・役割</dt>
  <dd>anchorの意味で、href属性を用いることでリンクを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ (hrefを指定した場合)</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>トランスペアレント<br>子孫にインタラクティブ・コンテンツの要素、a、tabindex属性が指定された要素は配置不可</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    href ・・・ リンクのアドレスを指定 (hypertext referenceの略)<br>
    target ・・・ リンク先を表示するタブまたはウインドウを指定<br>
    download ・・・ リンク先のファイルをダウンロードする<br>
    rel ・・・ リンク先との関係性
  </dd>
</dl>

### target 属性

| 属性値                 | 説明                               |
| ---------------------- | ---------------------------------- |
| \_self                 | 現在のウインドウまたはタブで表示   |
| \_parent               | 親のウインドウまたはタブで表示     |
| \_top                  | 最上位のウインドウまたはタブで表示 |
| \_blank                | 新しいウインドウまたはタブで表示   |
| ウインドウ名 or タブ名 | 指定したウインドウまたはタブで表示 |

### rel 属性

| 属性値     | 説明                                                   |
| ---------- | ------------------------------------------------------ |
| alternate  | モバイル専用サイトや別の言語ページなどを表す           |
| author     | 著者の詳しい情報のページを表す                         |
| bookmark   | 深く関係しているページを表す                           |
| noreferrer | リンク先にリンク元の情報を送らない + noopener の効果   |
| noopener   | リンク先からリンク元の情報にアクセスできないようにする |
| nofollow   | サイト管理者がリンク先を承認していないことを示す       |

他にも、google 向けにスポンサーを表す`sponsored`やユーザーが作成したコンテンツを表す`ufc`などがある。

### ページ内リンク

同一ページの異なる場所に遷移させる場合は次のようにする

```html
<!-- 遷移先 -->
<h2 id="food">フードメニュー</h2>

<!-- anchor (# + id) -->
<a href="#food">フード</a>

<!-- ページ先頭 -->
<a href="#top">ページ先頭へ</a>
```

## **[img](https://developer.mozilla.org/ja/docs/Web/HTML/Element/img)**

<dl>
  <dt>意味・役割</dt>
  <dd>imageの意味で、画像を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>エンベディット・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    src ・・・ 参照する画像のURLを指定<br>
    srcset ・・・ 解像度違いなど複数の画像ファイルを指定する (`url [デバイスピクセル比]x,`の形で指定)<br>
    alt ・・・ 画像の代替テキストを指定<br>
    width, height ・・・ 画像の横幅、縦幅 (px)<br>
    decoding ・・・ 画像のでコードのヒントを指定する<br>
    loading ・・・ 画像の読み込みタイミングを指定
  </dd>
</dl>

### alt 属性

置き換えてもページの意味が変わらないようなテキスト、装飾の場合は空を指定する。  
画像をリンクとして使用する場合は、空にならないように注意が必要

### decoding 属性

| 属性値 | 説明                   |
| ------ | ---------------------- |
| sync   | 同期的にデコードを行う |
| async  | 非同期でデコードを行う |
| auto   | 自動 (ブラウザによる)  |

### loading 属性

| 属性値 | 説明           |
| ------ | -------------- |
| lazy   | 遅延読み込み   |
| eager  | すぐに読み込み |

### **[picture](https://developer.mozilla.org/ja/docs/Web/HTML/Element/picture)**

デバイスや条件によって切り替える場合、`picture`タグを使用して次のように表すことができる

```html
<picture>
  <source srcset="URL" media="この画像になる条件(cssのmedia query)" />
  <img src="URL" alt="代替テキスト" />
</picture>
```

## **[video](https://developer.mozilla.org/ja/docs/Web/HTML/Element/video)**

<dl>
  <dt>意味・役割</dt>
  <dd>動画を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>エンベディット・コンテンツ<br>インタラクティブ・コンテンツ (controls属性がある場合)</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    srcがある・・・0個以上のtrack要素、メディア要素を含まないトランスペアレント<br>
    srcがない・・・0個以上のsource要素、0個以上のtrack要素、メディア要素を含まないトランスペアレント
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    src ・・・ 参照する動画のURLを指定<br>
    poster ・・・ ビデオが再生される前に表示される画像を指定<br>
    autoplay ・・・ 読み込まれた際に自動で再生するかを指定<br>
    playsinline ・・・ 動画を再生するブラウザに対してインラインで再生するようにする<br>
    loop ・・・ 動画を繰り返し再生するかを指定<br>
    muted ・・・ デフォルトでミュートにするかを指定<br>
    controls ・・・ 動画のコントローラーを表示するかを指定<br>
    width, height ・・・ 動画の横幅、縦幅 (px) を指定<br>
  </dd>
</dl>

### autoplay 属性

自動再生されることで予期せぬデータ通信が発生する可能性があるため、ユーザー自身で再生させることが推奨されています。スマートフォンでは`playsinline`を指定していないと自動再生されないため、使用する際は`muted`, `playsinline`, `controls`をセットで指定することが基本です。

### **[source](https://developer.mozilla.org/ja/docs/Web/HTML/Element/source)**

<dl>
  <dt>意味・役割</dt>
  <dd>複数の代替メディアファイルを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    src ・・・ 参照するファイルのURLを指定<br>
    type ・・・ ファイルの種類をMIMEで指定<br>
  </dd>
</dl>

### **[track](https://developer.mozilla.org/ja/docs/Web/HTML/Element/track)**

<dl>
  <dt>意味・役割</dt>
  <dd>字幕などのテキストトラックを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    src ・・・ 参照するファイルのURLを指定<br>
    kind ・・・ テキストトラックの種類を指定<br>
    srclang ・・・ テキストトラックの言語を指定　(kind属性が「subtitles」の場合は必須)<br>
    label ・・・ ユーザーに表示されるラベルを指定<br>
  </dd>
</dl>

#### kind 属性

| 属性値       | 説明                                                                           |
| ------------ | ------------------------------------------------------------------------------ |
| subtitles    | 字幕の意味で、会話などの文字お越しや翻訳したテキストトラック                   |
| captions     | 音声が利用できない場合や耳が不自由な方向けに非言語情報を含んだテキストトラック |
| descriptions | 動画が視聴できない場合や目が不自由な方向けに内容を説明したテキストトラック     |
| chapters     | チャプターごとのタイトルを記したテキストトラック                               |
| metadata     | JS 等からの利用を目的としたテキストトラック                                    |

## **[iframe](https://developer.mozilla.org/ja/docs/Web/HTML/Element/iframe)**

<dl>
  <dt>意味・役割</dt>
  <dd>inline frameの意味で、他のページのコンテンツを埋め込む。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>エンベディット・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>なし</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    src ・・・ 参照する動画のURLを指定<br>
    width, height ・・・ 動画の横幅、縦幅 (px) を指定<br>
    loading ・・・ 画像の読み込みタイミングを指定
  </dd>
</dl>

## **[figure](https://developer.mozilla.org/ja/docs/Web/HTML/Element/figure)**

<dl>
  <dt>意味・役割</dt>
  <dd>本文から切り離せるイラスト、図、写真、コードなどを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    1. figcaption要素とそれに続くフロー・コンテンツ<br>
    2. フロー・コンテンツとそれに続くfigcation要素<br>
    3. フロー・コンテンツ<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[figcaption](https://developer.mozilla.org/ja/docs/Web/HTML/Element/figcaption)**

<dl>
  <dt>意味・役割</dt>
  <dd>親のfigure要素内にあるコンテンツのキャプションや凡例を表す</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>
