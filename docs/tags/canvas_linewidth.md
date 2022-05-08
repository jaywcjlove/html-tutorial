HTML canvas lineWidth 属性
===

## 示例

绘制一个线宽为 10 像素的矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML5 canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.lineWidth = 10;
ctx.strokeRect(20, 20, 80, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.lineWidth = 10;
ctx.strokeRect(20, 20, 80, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| lineWidth | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

lineWidth 属性设置或返回当前线宽，以像素为单位。

| 默认值:     | `1` |
| ----------- | ----------- |
| JavaScript 语法: | *context*.lineWidth=*number*; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value  | 描述 Description |
| ------ | ------ |
| *number* | 当前线宽，以像素为单位 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
