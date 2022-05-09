HTML `id` 属性
===

## 实例

使用 `id` 属性通过 JavaScript 操作文本：

```html idoc:preview:iframe
<h2 id="myHeader">Hello World!</h2>
<button onclick="displayResult()">Change text</button>
<script>
function displayResult() {
  document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script>
```

## 定义和使用

`id` 属性为 HTML 元素指定一个唯一的 id（该值在 HTML 文档中必须是唯一的）。

`id` 属性最常用于指向样式表中的样式，并通过 JavaScript（通过 HTML DOM）来操作具有特定 `id` 的元素。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;id&gt;__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element id="id">
```

## 属性值

值 Value | 描述 Description
---- | ----
id | 指定元素的唯一 ID。 命名规则：<br/>1. 必须包含至少一个字符<br/> 2. 不得包含任何空格字符
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg