HTML canvas arcTo() 方法
===

## 示例

在画布上的两条切线之间创建圆弧：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);               // 创建起点
ctx.lineTo(100, 20);              // 创建水平线
ctx.arcTo(150, 20, 150, 70, 50);  // 创建圆弧
ctx.lineTo(150, 120);             // 继续垂直线
ctx.stroke();                     // 画出来
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);               // 创建起点
ctx.lineTo(100, 20);              // 创建水平线
ctx.arcTo(150, 20, 150, 70, 50);  // 创建圆弧
ctx.lineTo(150, 120);             // 继续垂直线
ctx.stroke();                     // 画出来
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| `arcTo()` | Yes | 9.0 | Yes | Yes | No |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`arcTo()` 方法在画布上的两条切线之间创建弧/曲线。

![画布 arcto() 图](../assets/img_canvas_arcto.png)

**提示：** 使用 [stroke()](canvas_stroke.md) 方法在画布上实际绘制弧线。

| JavaScript 语法: | *context*.arcTo(*x1,y1,x2,y2,r*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x1*  | 第一条切线的 x 坐标 | 
| *y1*  | 第一个切线的 y 坐标 | 
| *x2*  | 第二个切线的 x 坐标 | 
| *y2*  | 第二个切线的 y 坐标 | 
| *r*   | 圆弧的半径 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg