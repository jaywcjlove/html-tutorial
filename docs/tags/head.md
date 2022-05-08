HTML \<head> 标签
===

## 示例

一个简单的 HTML 文档，在 head 部分带有 [\<title>](./title.md) 标记：

```html idoc:preview:iframe
<!DOCTYPE html>
<html lang="en">
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

`<head>` 元素是元数据（关于数据的数据）的容器，位于 [\<html>](./html.md) 标签和 [\<body>](./body.md) 标签之间。

元数据是关于 HTML 文档的数据。 不显示元数据。

元数据通常定义文档标题、字符集、样式、脚本和其他元信息。

以下元素可以进入 `<head>` 元素：

* [\<title>](./title.md) （每个 HTML 文档都需要）
* [\<style>](./style.md)
* [\<base>](./base.md)
* [\<link>](./link.md)
* [\<meta>](./meta.md)
* [\<script>](./script.md)
* [\<noscript>](./noscript.md)

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<head> | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<head>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 更多示例

[\<base>](./base.md) 标记（指定页面上所有链接的默认 URL 和目标）位于 \<head> 内：

```html idoc:preview:iframe
<html>
<head>
  <base href="https://wangchujiang.com/" target="_blank">
</head>
<body>
    <img src="html-tutorial/assets/chrome.svg" width="24" height="39" alt="chrome">
    <a href="html-tutorial/base.html">HTML base Tag</a>
</body>
</html>
```

[\<style>](./style.md) 标记（将样式信息添加到页面）进入 \<head>：

```html idoc:preview:iframe
<html>
<head>
  <style>
    h1 {color:red;}
    p {color:blue;}
  </style>
</head>
<body>
  <h1>A heading</h1>
  <p>A paragraph.</p>
</body>
</html>
```

[\<link>](./link.md) 标记（链接到外部样式表）进入 \<head>：

```html idoc:preview:iframe
<html>
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
  <h1>I am formatted with a linked style sheet</h1>
  <p>Me too!</p>
</body>
</html>
```

## 相关页面

HTML tutorial: [HTML Head](../tutorial/head.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<head>` 元素：

```css
head {
  display: none;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg