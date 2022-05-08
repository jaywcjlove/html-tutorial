HTML canvas lineJoin 属性
===

## 示例

当两条线相交时创建一个圆角：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML5 canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.lineWidth = 10;
ctx.lineJoin = "round";
ctx.moveTo(20, 20);
ctx.lineTo(100, 50);
ctx.lineTo(20, 100);
ctx.stroke();
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.lineJoin = "round";
ctx.moveTo(20, 20);
ctx.lineTo(100, 50);
ctx.lineTo(20, 100);
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| lineJoin | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`lineJoin` 属性设置或返回两条线相交时创建的角的类型。

**注意：** “miter”值受 [miterLimit](canvas_miterlimit.md) 属性的影响。

| 默认值: | `miter` |
| ----------- | ----------- |
| JavaScript syntax: | *context*.lineJoin="bevel/round/miter"; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value  | 描述 Description |
| ------ | ------ |
| bevel | 创建斜角 |
| round | 创建圆角 |
| miter | 默认。 创建一个尖角 |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

