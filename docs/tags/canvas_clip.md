HTML canvas clip() 方法
===

## 示例

从画布上截取一个 200*120 像素的矩形区域。 然后，绘制一个红色矩形。 只有裁剪区域内的红色矩形部分可见：

```html idoc:preview:iframe
<div>Without clip():</div>
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 画一个矩形
ctx.rect(50, 20, 200, 120);
ctx.stroke();
// 绘制红色矩形
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 150, 100);
</script> 

<div>With clip():</div>
<canvas id="myCanvas2" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas2");
var ctx = c.getContext("2d");
// 裁剪一个矩形区域
ctx.rect(50, 20, 200, 120);
ctx.stroke();
ctx.clip();
// 绘制红色矩形 after clip()
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 裁剪一个矩形区域
ctx.rect(50, 20, 200, 120);
ctx.stroke();
ctx.clip();
// 在 clip() 之后绘制红色矩形
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| clip() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`clip()` 方法从原始画布中裁剪出任意形状和大小的区域。

**提示：** 一旦某个区域被剪裁，以后的所有绘图都将被限制在剪裁区域内（无法访问画布上的其他区域）。 但是，您可以在使用 clip() 方法之前使用 save() 方法保存当前画布区域，并在将来的任何时间恢复它（使用 restore() 方法）。

| JavaScript 语法: | *context*.clip(); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
