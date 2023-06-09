# 表とフォームを作ろう

## **[table](https://developer.mozilla.org/ja/docs/Web/HTML/Element/table)**

<dl>
  <dt>意味・役割</dt>
  <dd>表を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    1. 任意でcaption要素<br>
    2. 任意でthead要素<br>
    3. それに続く0個以上のtbody or 1つ以上のtr<br>
    4. 任意でtfoot要素<br>
    5. 任意でスクリプトサポーティング要素<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[tr](https://developer.mozilla.org/ja/docs/Web/HTML/Element/tr)**

<dl>
  <dt>意味・役割</dt>
  <dd>table rowの意味で、表の中の行を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>0個以上のth, td要素, スクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[th](https://developer.mozilla.org/ja/docs/Web/HTML/Element/th)**

<dl>
  <dt>意味・役割</dt>
  <dd>tableのheader cellの意味で、見出しのセルを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ<br>ただし、子孫にheader, footer, セクショニング・コンテンツ, ヘディング・コンテンツは配置不可</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    scope・・・見出しの対象範囲を指定する<br>
    rowspan・・・行の結合する数を指定する<br>
    colspan・・・列の結合する数を指定する<br>
  </dd>
</dl>

#### scope 属性

| 属性値   | 説明                                 |
| -------- | ------------------------------------ |
| row      | 同じ行のセルがこの見出しの対象       |
| col      | 同じ列のセルがこの見出しの対象       |
| rowgroup | 行グループ内のセルがこの見出しの対象 |
| colgroup | 列グループ内のセルがこの見出しの対象 |

### **[td](https://developer.mozilla.org/ja/docs/Web/HTML/Element/td)**

<dl>
  <dt>意味・役割</dt>
  <dd>tableのdata cellの意味で、内容のセルを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    rowspan・・・行の結合する数を指定する<br>
    colspan・・・列の結合する数を指定する<br>
  </dd>
</dl>

### **[caption](https://developer.mozilla.org/ja/docs/Web/HTML/Element/caption)**

<dl>
  <dt>意味・役割</dt>
  <dd>表のキャプションを表す</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[thead](https://developer.mozilla.org/ja/docs/Web/HTML/Element/thead)**

<dl>
  <dt>意味・役割</dt>
  <dd>table　headerの意味で、見出し行を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>０個以上のtr要素とスクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[tbody](https://developer.mozilla.org/ja/docs/Web/HTML/Element/tbody)**

<dl>
  <dt>意味・役割</dt>
  <dd>table　bodyの意味で、内容部分の行を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>０個以上のtr要素とスクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

### **[tfoot](https://developer.mozilla.org/ja/docs/Web/HTML/Element/tfoot)**

<dl>
  <dt>意味・役割</dt>
  <dd>table　footerの意味で、フッター行を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>０個以上のtr要素とスクリプトサポーティング要素</dd>
  <dt>利用できる属性</dt>
  <dd>グローバル属性</dd>
</dl>

## **[form](https://developer.mozilla.org/ja/docs/Web/HTML/Element/form)**

<dl>
  <dt>意味・役割</dt>
  <dd>フォームを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    フロー・コンテンツ (子孫にformは配置不可)<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    action・・・送信先を指定する<br>
    method・・・送信方法を指定する (get / post / dialog)<br>
    enctype・・・送信形式を指定する
  </dd>
</dl>

### name

formData として扱うために、子孫の input 要素には`name`属性を指定するようにする

## **[input](https://developer.mozilla.org/ja/docs/Web/HTML/Element/input)**

<dl>
  <dt>意味・役割</dt>
  <dd>フォームのコントロール部分を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    なし<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    type ・・・ 部品の種類を指定する<br>
    name ・・・ 部品の名前を指定する<br>
    value ・・・ 部品の値を指定する<br>
    size ・・・ 部品の幅を文字数で指定する (init: 20)<br>
    maxlength ・・・ 入力できる最大文字数を指定する<br>
    checked ・・・ 選択状態にする (typeがcheckbox or radioのとき)<br>
    placeholder ・・・ 部品内に表示されるヒントを指定する<br>
    required ・・・ 入力を必須にする<br>
    autocomplete ・・・ 入力の自動保管に関するヒントを提供する<br>
    readonly ・・・ 部品を読み取り専用にする<br>
    disabled ・・・ 部品を無効にする<br>
  </dd>
</dl>

### type 属性

【入力系】<br>text, password, tel, url, email, search, datetime-local, date, month, week, time, number, range, color

【選択系】<br>radio, checkbox (`name`属性を指定することで同じまとまりに指定できる)

【ボタン系】<br>submit, reset, button, image, file

【その他】<br>hidden

## **[button](https://developer.mozilla.org/ja/docs/Web/HTML/Element/button)**

<dl>
  <dt>意味・役割</dt>
  <dd>ボタンを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    フロー・コンテンツ (子孫にインタラクティブ・コンテンツ, tabindexが指定された要素は配置不可)<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    type ・・・ 種類を指定する (submit / reset / button)<br>
    name ・・・ ボタンの名前を指定する<br>
  </dd>
</dl>

## **[textarea](https://developer.mozilla.org/ja/docs/Web/HTML/Element/textarea)**

<dl>
  <dt>意味・役割</dt>
  <dd>複数行の入力フィールドを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    テキスト(初期値として使用される)<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    name ・・・ 部品の名前を指定する<br>
    cols ・・・ 1行あたりの最大文字数を指定する<br>
    rows ・・・ 表示する行数を指定する<br>
    maxlength ・・・ 入力できる最大文字数を指定する<br>
    placeholder ・・・ 部品内に表示されるヒントを指定する<br>
    required ・・・ 入力を必須にする<br>
  </dd>
</dl>

## **[select](https://developer.mozilla.org/ja/docs/Web/HTML/Element/select)**

<dl>
  <dt>意味・役割</dt>
  <dd>セレクトボックスを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    0個以上のoption, optgroup, スクリプトサポーティング要素<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    name ・・・ 部品の名前を指定する<br>
    multiple ・・・ 複数の値を選択可能にする<br>
    required ・・・ 入力を必須にする<br>
  </dd>
</dl>

### **[option](https://developer.mozilla.org/ja/docs/Web/HTML/Element/option)**

<dl>
  <dt>意味・役割</dt>
  <dd>セレクトボックスの選択肢, 入力を補完する候補を表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    label: 指定, value: 指定 ・・・ 空<br>
    label: 指定, value: 未指定 ・・・ テキスト<br>
    label: 未指定, datelistの子要素でない ・・・ 空白ではないテキスト<br>
    label: 未指定, datelistの子要素である ・・・ テキスト<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    label ・・・ ユーザーに表示するラベルを指定する<br>
    selected ・・・ 選択状態にする<br>
    value ・・・ 送信される値を指定する<br>
  </dd>
</dl>

### **[optgroup](https://developer.mozilla.org/ja/docs/Web/HTML/Element/optgroup)**

<dl>
  <dt>意味・役割</dt>
  <dd>セレクトボックスの選択肢のグループを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>なし</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    0個以上のoption, スクリプトサポーティング要素<br>
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    label ・・・ ユーザーに表示するラベルを指定する<br>
  </dd>
</dl>

### **[label](https://developer.mozilla.org/ja/docs/Web/HTML/Element/label)**

<dl>
  <dt>意味・役割</dt>
  <dd>コントロール部分のラベルを表す。</dd>
  <dt>カテゴリ</dt>
  <dd>フロー・コンテンツ<br>フレージング・コンテンツ<br>インタラクティブ・コンテンツ</dd>
  <dt>コンテンツ・モデル(内包可能な要素)</dt>
  <dd>
    フレージング・コンテンツ(子孫にlabelは配置不可)<br>
    button, input( type != hidden ), meter, output, progress, select, textarea, フォームに関連付けられたカスタム要素以外のコントロール要素は配置不可
  </dd>
  <dt>利用できる属性</dt>
  <dd>
    グローバル属性<br>
    for ・・・ ラベルと関連するコントロール部分を指定する<br>
  </dd>
</dl>

### 記述例

```html
<!-- 記法1 -->
<label> お名前: <input type="text" name="your_name" /> </label>

<!-- 記法2 -->
<label for="name">お名前:</label>
<input type="text" name="your_name" id="name" />
```
