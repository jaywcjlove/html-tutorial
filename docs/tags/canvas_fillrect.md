HTML canvas fillRect() 方法
===

## 示例

绘制一个填充的 150\*100 像素矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillRect(20, 20, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| fillRect() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`fillRect()` 方法绘制一个“填充”矩形。 填充的默认颜色是黑色。

**提示：** 使用 [fillStyle](canvas_fillstyle.md) 属性设置用于填充绘图的颜色、渐变或图案。

| JavaScript 语法: | *context*.fillRect(*x,y,width,height*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x*       | 矩形左上角的 x 坐标 |
| *y*       | 矩形左上角的 y 坐标 |
| *width*   | 矩形的宽度，以像素为单位 |
| *height*  | 矩形的高度，以像素为单位 |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg