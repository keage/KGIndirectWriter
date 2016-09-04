# KGIndirectWriter

## 概要

DirectWrite 環境のブラウザで発生する AA のズレを調整するスクリプト

**AA 用なので 16px MS Pゴシックの使用が前提です**

<figure>
  <img src="http://keage.tokyo/AA/KGIW-before.png" alt="邪気眼を持たざる者 (KGIndirectWriter 使用前)">
  <figcaption>KGIndirectWriter 使用前</figcaption>
</figure>
<figure>
  <img src="http://keage.tokyo/AA/KGIW-after.png" alt="邪気眼を持ちし者 (KGIndirectWriter 使用後)">
  <figcaption>KGIndirectWriter 使用後</figcaption>
</figure>

## 使い方

KGIndirectWriter.min.js をダウンロード & 自サイトにアップロードし、以下のコードをブログテンプレの<s> head 末尾か</s> body 末尾に追加

_2016/09/04 追記： head 末尾へのスクリプト追加はエラーが発生しましたので body 末尾への追加でお願いします。_

````
<script src="[アップロード先の URL]"></script>
<script>KGIndirectWriter.process("[AA が存在する要素の CSS セレクタ]")</script> 
````

_CSS セレクタについての詳しい情報は [MDN のドキュメント](https://developer.mozilla.org/ja/docs/Web/CSS/Reference#Selectors) をご覧ください。_

### 例

- アップロード先の URL: `http://example.com/js/KGIndirectWriter.min.js`
- AA が存在する要素: `class="aa"` を指定した要素すべて

の場合：

````
<script src="http://example.com/js/KGIndirectWriter.min.js"></script>
<script>KGIndirectWriter.process(".aa")</script> 
````

## ライセンス

The MIT License (MIT)
Copyright (c) 2016 YAMASINA Keage <[@keag](https://twitter.com/keage)[e](https://alpha.app.net/keage)>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
