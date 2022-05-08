HTML canvas stroke() 方法
===

## 示例

绘制一条路径，形状为字母 L - 红色：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.beginPath();
  ctx.moveTo(20, 20);
  ctx.lineTo(20, 100);
  ctx.lineTo(70, 100);
  ctx.strokeStyle = "red";
  ctx.stroke();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.lineTo(20, 100);
ctx.lineTo(70, 100);
ctx.strokeStyle = "red";
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| stroke() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


## 定义和用法

`stroke()` 方法实际上绘制了您使用所有这些 `moveTo()` 和 `lineTo()` 方法定义的路径。 默认颜色为黑色。

**提示：** 使用 [strokeStyle](canvas_strokestyle.md) 属性以其他颜色/渐变进行绘制。

| JavaScript 语法: | *context*.stroke(); |
| -------- | -------- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
