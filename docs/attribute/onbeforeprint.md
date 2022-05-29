HTML onbeforeprint 属性
===

## 定义和用法

`onbeforeprint` 属性在页面即将被打印时触发（在打印对话框出现之前）。

**提示：** `onbeforeprint` 属性通常与 `onafterprint` 属性一起使用。

## 适用于

`onbeforeprint` 属性是 [事件属性](../reference/eventattributes.md) 的一部分，可用于以下元素：

| 元素 | 事件 |
| --- | --- |
| [\<body>](../tags/body.md) | [onbeforeprint](../attribute/onbeforeprint.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

在即将打印页面时执行 JavaScript：

```html idoc:preview:iframe
<body onbeforeprint="myFunction()">

<h1>尝试打印此文档</h1>
<p><b>提示:</b> 键盘快捷键，例如 Ctrl+P/Command+P 设置要打印的页面。</p>
<p><b>注意:</b> Safari 和 Opera 不支持 onbeforeprint 事件。</p>

<script>
function myFunction() {
  alert("You are about to print this document!");
}
</script>
</body>
```

## 浏览器支持

表中的数字指定了完全支持该事件的第一个浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onbeforeprint   | 63 | Yes | Yes | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
