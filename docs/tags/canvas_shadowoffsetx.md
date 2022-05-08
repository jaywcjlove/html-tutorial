HTML canvas shadowOffsetX 属性
===

## 示例

绘制一个阴影放置在右侧 20 像素的矩形（从矩形的左侧位置开始）：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.shadowBlur = 10;
ctx.shadowOffsetX = 20;
ctx.shadowColor = "black";
ctx.fillStyle= "red";
ctx.fillRect(20, 20, 100, 80);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.shadowBlur = 10;
ctx.shadowOffsetX = 20;
ctx.shadowColor = "black";
ctx.fillStyle = "red";
ctx.fillRect(20, 20, 100, 80);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| shadowOffsetX | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`shadowOffsetX` 属性设置或返回阴影与形状的水平距离。

`shadowOffsetX=0` 表示阴影就在形状的后面。

`shadowOffsetX=20` 表示阴影从右侧开始 20 个像素（从形状的左侧位置开始）。

`shadowOffsetX=-20` 表示阴影从左侧 20 像素处开始（从形状的左侧位置开始）。

**提示：** 要调整阴影与形状的垂直距离，请使用 [shadowOffsetY](canvas_shadowoffsety.md) 属性。

| 默认值: | `0` |
| ------- | ------- |
| JavaScript 语法: | *context*.shadowOffsetX=*number*; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | 定义阴影与形状的水平距离的正数或负数 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg