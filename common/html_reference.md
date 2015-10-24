# HTMLリファレンス
## HTMLとは

HTML（HyperText Markup Language）とは、webサイトを作成するために開発された言語です。現在インターネット上で公開されているwebサイトのほとんどがhtmlで書かれてます。タグを複数組み合わせることでサイトを構築していきます。


## タグ一覧

### `<!DOCTYPE html>` *必須*

htmlのバージョンを宣言しています。上記の書き方は、html5を使用することを示しています。今後はhtml5が主流になっていくので、これを覚えておけば問題ないと思います。

### `<html>...</html>` *必須*

その文章がhtmlであることを宣言しています。全体をこのタグで囲むと覚えておきましょう。

### `<head>...</head>` *必須*

htmlの設定をここに書きます。タイトルを設定したり、スタイルシートの読み込み、スクリプトの読み込みなどを行います。

### `<title>...</title>`

webサイトのタイトルを設定します。タイトルを書くと、ブラウザのタブにそれが表示されます。

#### 記述例

```html
<title>Google</title>
```

以下のように表示されます。

![titleの例](images/html_reference/title.png)

### `<meta charset="utf-8">`

文字コードの設定を行います。utf-8は日本語に対応しているので、webサイト上で日本語を使用する場合は指定します。

### `<link rel="stylesheet" href="...">`

スタイルシート（文字色・サイズなどの装飾）を読み込みます。`href`にはファイル名（例えば、`style.css`）を指定します。

### `<body>...</body>` *必須*

本文（文章・画像）を記述します。body内に書いたものがwebサイト上に表示されます。

### `<div>...</div>`

divisionの略で、分割された区分
これ自体に意味はないのですが、最もよく使うタグです。スタイルシートで大きさや位置を決め、レイアウトを構成します。

### `<p>...</p>`

パラグラフ（Paragraph）のPで段落を示します。文章のまとまりが複数あった場合、それぞれをpタグで囲みます。

### `<a href="...">...</a>`

リンクを設定できます。`href`には、リンク先のURLまたはファイル名を指定し、タグの間にリンクのテキストを書きます。

#### 記述例

```html
<a href="test.html">テストページへのリンク</a>
<a href="http://doshisha.ac.jp">同志社大学</a>
```

### `<h1>...</h1>`

文章の見出しを示します。`<h1>`を最上位に`<h6>`を最も低いレベルとする6段階で書くことができます。

#### 記述例

```html
<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>
```

以下のように表示されます。

![titleの例](images/html_reference/hx.png)

### `<img src="...">`

画像を表示します。`src`に画像のファイル名またはURLを指定します。

### `<ul>...</ul>`


リストを作る際に使用します。中に`<li>`タグを伴って使います。

#### 記述例

```html
<ul>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ul>
```

以下のように表示されます。

![titleの例](images/html_reference/list.png)

### `<!-- ... -->`

コメントです。この間に書かれた文字はwebサイトには表示されません。プログラムの意味など注釈に使用します。


## 用語

### タグ

タグとは、`<title>`のように、`<>`で囲まれたものを指します。基本的に、開始タグと終了タグが対になっていて、`<title>中身</title>`のように使います。

### 属性

属性は、タグの役割や値を指定するために使用します。属性は開始タグの中に書きます。

```html
<a href="http://doshisha.ac.jp">同志社</a>
```

この例では、`href`が属性に当たり、値が`http://doshisha.ac.jp`となります。ちなみに、hrefはHyperText Referenceの略で、"参照先"という意味です。つまり、リンクの参照先を同志社のwebサイトにする、という意味です。

### id

スタイルシートやJavaScriptにおいて、タグを特定するために使用します。同じhtml内で同一のidは使用できません。

### class

スタイルシートやJavaScriptにおいて、タグを特定するために使用します。idと違い、同一classは複数回使用できます。
