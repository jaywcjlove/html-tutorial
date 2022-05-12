HTML onscroll 事件属性
===

滚动元素的滚动条时运行的脚本

## 示例

在滚动 [\<div>](../tags/div.md) 元素时执行 JavaScript：

```html
<div onscroll="myFunction()">
```

```html idoc:preview:iframe
<style>
  #myDIV {
    border: 1px solid black;
    width: 200px;
    height: 100px;
    overflow: scroll;
  }
</style>
</head>
<body>

<p>试试 div 中的滚动条。</p>

<div id="myDIV" onscroll="myFunction()">
HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）。
<br><br>
“超文本”（hypertext）是指连接单个网站内或多个网站间的网页的链接。链接是网络的一个基本方面。只要将内容上传到互联网，并将其与他人创建的页面相链接，你就成为了万维网的积极参与者。
<br><br>
HTML 使用“标记”（markup）来注明文本、图片和其他内容，以便于在 Web 浏览器中显示。</div>
<script>
function myFunction() {
  document.getElementById("myDIV").style.color = "red";
}
</script>
<p>当您在 div 中滚动时会触发一个函数。 该函数将 div 中文本的颜色设置为红色。</p>
```

## 定义和使用

`onscroll` 属性在元素的滚动条被滚动时触发。

**提示：** 使用 CSS `overflow` 样式属性为元素创建滚动条。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onscroll        | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onscroll="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 `onscroll` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<address>](../tags/address.md), [\<blockquote>](../tags/blockquote.md), [\<body>](../tags/body.md), [\<caption>](../tags/caption.md), [\<center>](../tags/center.md), [\<dd>](../tags/dd.md), [\<dir>](../tags/dir.md), [\<div>](../tags/div.md), [\<dl>](../tags/dl.md), [\<dt>](../tags/dt.md), [\<fieldset>](../tags/fieldset.md), [\<form>](../tags/form.md), [\<h1>](../tags/hn.md) ~ [\<h6>](../tags/hn.md), [\<html>](../tags/html.md), [\<li>](../tags/li.md), [\<menu>](../tags/menu.md), [\<object>](../tags/object.md), [\<ol>](../tags/ol.md), [\<p>](../tags/p.md), [\<pre>](../tags/pre.md), [\<select>](../tags/select.md), [\<tbody>](../tags/tbody.md), [\<textarea>](../tags/textarea.md), [\<tfoot>](../tags/tfoot.md), [\<thead>](../tags/thead.md), [\<ul>](../tags/ul.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


