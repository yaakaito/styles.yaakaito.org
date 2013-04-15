---
---

# DOM要素を作成する関数名

`createDOM`をプレフィックスとして付けます。`make`や`create`と書いてはいけません。
冗長ですが、統一をもたらす為に必要な要素です。

# JavaScriptから利用するDOMに対するネーミング

## id

idはJavaScriptからのアクセスを行うためのみに利用します。
CSSでidを利用したスタイル指定を行ってはいけません。
大文字から始まるキャメルケースで記述します。

```html
<div id="ForJavaScript"></div>
```

## class

JavaScriptから利用するclassには`js-`をプレフィックスとして記述します。
ハイフンつなぎで記述します。

```html
<div class="js-for-js-class for-css-class">
```


