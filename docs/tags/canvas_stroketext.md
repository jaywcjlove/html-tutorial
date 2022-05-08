HTML canvas strokeText() 方法
===

## 示例

写“Hello world!” 和“Big smile!” （带渐变）在画布上，使用 `strokeText()`：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.font = "20px Georgia";
ctx.strokeText("Hello World!", 10, 50);

ctx.font = "30px Verdana";
// 创建渐变

var gradient = ctx.createLinearGradient(0, 0, c.width, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5", "blue");
gradient.addColorStop("1.0", "red");

// 填充渐变
ctx.strokeStyle = gradient;
ctx.strokeText("Big smile!", 10, 90);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.font = "20px Georgia";
ctx.strokeText("Hello World!", 10, 50);

ctx.font = "30px Verdana";
// 创建渐变

var gradient = ctx.createLinearGradient(0, 0, c.width, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5", "blue");
gradient.addColorStop("1.0", "red");

// 填充渐变
ctx.strokeStyle = gradient;
ctx.strokeText("Big smile!", 10, 90);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| `strokeText()` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** Safari 5.1 及更早版本不支持 maxWidth 参数。

## 定义和用法

`strokeText()` 方法在画布上绘制文本（没有填充）。 文本的默认颜色是黑色。

**提示：** 使用 [font](canvas_font.md) 属性指定字体和字体大小，并使用 [strokeStyle](canvas_strokestyle.md) 属性以另一种颜色/渐变呈现文本。

| JavaScript syntax: | *context*.strokeText(*text,x,y,maxWidth*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *text*     | 指定将在画布上写入的文本 |
| *x*        | 开始绘制文本的 x 坐标（相对于画布） |
| *y*        | y 坐标开始绘制文本的位置（相对于画布） |
| *maxWidth* | 选修的。 文本的最大允许宽度，以像素为单位 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

