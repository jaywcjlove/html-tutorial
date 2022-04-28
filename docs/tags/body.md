HTML \<body> Tag
===

## 示例

一个简单的 HTML 文档：

```html idoc:preview:iframe
<html>
<head>
  <title>Title of the document</title>
</head>
<body>
  <h1>This is a heading</h1>
  <p>This is a paragraph.</p>
</body>
</html>
```

## 定义和用法

`<body>` 标签定义了文档的正文。

`<body>` 元素包含 HTML 文档的所有内容，例如标题、段落、图像、超链接、表格、列表等。

**注意：** HTML 文档中只能有一个 `<body>` 元素。

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<body> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<body>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<body>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

将背景图像添加到文档（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    body {
      background-image: url(good.png);
    }
  </style>
</head>
<body>
  <h1>Hello world!</h1>
  <p><a href="https://jaywcjlove.github.io/html-tutorial">HTML Tutorial!</a></p>
</body>
```

设置文档的背景颜色（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
<style>
  body {
    background-color: #E6E6FA;
  }
</style>
</head>
<body>
  <h1>Hello world!</h1>
  <p><a href="https://jaywcjlove.github.io/html-tutorial">HTML Tutorial!</a></p>
</body>
```

设置文档中文本的颜色（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    body {
      color: green;
    }
  </style>
</head>
<body>
  <h1>Hello world!</h1>
  <p>This is some text.</p>
  <p><a href="https://jaywcjlove.github.io/html-tutorial">HTML Tutorial!</a></p>
</body>
</html>
```

设置文档中未访问链接的颜色（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    a:link { color:#0000FF; }
  </style>
</head>
<body>
  <p><a href="https://jaywcjlove.github.io/html-tutorial/html/">HTML Tutorial</a></p>
</body>
</html>
```

设置文档中活动链接的颜色（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    a:active { color:#00FF00; }
  </style>
</head>
<body>
  <p><a href="https://jaywcjlove.github.io/html-tutorial/html/">HTML Tutorial</a></p>
</body>
</html>
```

设置文档中访问链接的颜色（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    a:visited { color:#FF0000; }
  </style>
</head>
<body>
  <p><a href="https://jaywcjlove.github.io/html-tutorial/html/">HTML Tutorial</a></p>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<body>` 元素：

```css
body {
  display: block;
  margin: 8px;
}
body:focus {
  outline: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg