HTML canvas lineCap 属性
===

## 示例

用圆形端盖画一条线：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");

  ctx.beginPath();
  ctx.lineWidth = 10;
  ctx.lineCap = "butt";
  ctx.moveTo(20, 20);
  ctx.lineTo(200, 20);
  ctx.stroke();

  ctx.beginPath();
  ctx.lineCap = "round";
  ctx.moveTo(20, 40);
  ctx.lineTo(200, 40);
  ctx.stroke();

  ctx.beginPath();
  ctx.lineCap = "square";
  ctx.moveTo(20, 60);
  ctx.lineTo(200, 60);
  ctx.stroke();
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.lineCap = "round";
ctx.moveTo(20, 20);
ctx.lineTo(200, 20);
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| lineCap  | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

lineCap 属性设置或返回线的端盖样式。

**注意：** 值 `round` 和 `square` 使线条略长。

| 默认值:     | `butt` |
| ----------- | ----------- |
| JavaScript 语法: | *context*.lineCap="`butt`/`round`/`square`"; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value  | 描述 Description |
| ------ | ------ |
| butt   | 默认。 一条平边被添加到线的每一端 |
| round  | 将圆形端盖添加到行的每一端 |
| square | 一个方形端盖被添加到该行的每一端 |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
