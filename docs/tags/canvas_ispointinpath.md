HTML canvas isPointInPath() 方法
===

## 示例

如果点 `20,50` 在当前路径中，则绘制一个矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML5 canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.rect(20, 20, 150, 100);
if (ctx.isPointInPath(20, 50)) {
  ctx.stroke();
};
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.rect(20, 20, 150, 100);
if (ctx.isPointInPath(20, 50)) {
  ctx.stroke();
};
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| `isPointInPath()` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

如果指定点在当前路径中，`isPointInPath()` 方法返回 `true`，否则返回 `false`。

| JavaScript syntax: | *context*.isPointInPath(*x,y*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x*       | 要测试的 x 坐标 |
| *y*       | 要测试的 y 坐标 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
