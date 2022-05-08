HTML canvas clearRect() 方法
===

## 示例

清除给定矩形内的一个矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 300, 150);
ctx.clearRect(20, 20, 100, 50);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 300, 150);
ctx.clearRect(20, 20, 100, 50);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| clearRect() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`clearRect()` 方法清除给定矩形内的指定像素。

| JavaScript 语法: | *context*.clearRect(*x,y,width,height*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x*       | 要清除的矩形左上角的 x 坐标 |
| *y*       | 要清除的矩形左上角的 y 坐标 |
| *width*   | 要清除的矩形的宽度，以像素为单位 |
| *height*  | 要清除的矩形的高度，以像素为单位 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
