HTML canvas shadowColor 属性
===

## 示例

绘制一个带有黑色阴影的红色矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.shadowBlur = 20;
ctx.fillStyle = "red";

ctx.shadowColor = "black";
ctx.fillRect(20, 20, 100, 80);

ctx.shadowColor = "blue";
ctx.fillRect(140, 20, 100, 80);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.shadowBlur = 20;
ctx.shadowColor = "black";
ctx.fillStyle = "red";
ctx.fillRect(20, 20, 100, 80);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| shadowColor | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`shadowColor` 属性设置或返回用于阴影的颜色。

**注意：** 使用 shadowColor 属性和 [shadowBlur](canvas_shadowblur.md) 属性来创建阴影。

**提示：** 使用 [shadowOffsetX](canvas_shadowoffsetx.md) 和 [shadowOffsetY](canvas_shadowoffsety.md) 属性调整阴影。

| 默认值: | `#000000` |
| ------- | ------- |
| JavaScript 语法: | *context*.shadowColor=*color*; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *color* | 用于阴影的 [CSS 颜色值](../reference/colornames.md)。 默认值为 `#000000` |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg