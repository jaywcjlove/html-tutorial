HTML canvas measureText() 方法
===

## 示例

在画布上写之前检查文本的宽度：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
var txt = "Hello World"
ctx.fillText("width:" + ctx.measureText(txt).width, 10, 50);
ctx.fillText(txt, 10, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
var txt = "Hello World"
ctx.fillText("width:" + ctx.measureText(txt).width, 10, 50)
ctx.fillText(txt, 10, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| measureText() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`measureText()` 方法返回一个对象，该对象包含指定文本的宽度（以像素为单位）。

**提示：** 如果您需要在将文本写入画布之前知道文本的宽度，请使用此方法。

| JavaScript 语法: | *context*.measureText(*text*).width; |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *text*    | 要测量的文本 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
