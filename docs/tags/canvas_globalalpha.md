HTML canvas globalAlpha 属性
===

## 示例

首先，绘制一个红色矩形，然后设置透明度（globalAlpha）为0.5，然后绘制一个蓝色和一个绿色矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(20, 20, 75, 50);

// 打开透明度
ctx.globalAlpha = 0.2;
ctx.fillStyle = "blue"; 
ctx.fillRect(50, 50, 75, 50); 
ctx.fillStyle = "green"; 
ctx.fillRect(80, 80, 75, 50);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(20, 20, 75, 50);

// 打开透明度
ctx.globalAlpha = 0.2;
ctx.fillStyle = "blue";
ctx.fillRect(50, 50, 75, 50);
ctx.fillStyle = "green";
ctx.fillRect(80, 80, 75, 50);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| globalAlpha | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| font        | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`globalAlpha` 属性设置或返回绘图的当前 `alpha` 或透明度值。

`globalAlpha` 属性值必须是介于 `0.0`（完全透明）和 `1.0`（不透明）之间的数字。

| 默认值: | `1.0` |
| ----- | ----- |
| JavaScript 语法: | *context*.globalAlpha=*number*; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value  | 描述 Description |
| ------ | ------ |
| *number* | 透明度值。 必须是介于 0.0（完全透明）和 1.0（不透明）之间的数字 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
