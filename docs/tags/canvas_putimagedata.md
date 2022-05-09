HTML canvas putImageData() 方法
===

## 示例

下面的代码使用 [`getImageData()`](./canvas_getimagedata.md) 复制画布上指定矩形的像素数据，然后使用 `putImageData()` 将图像数据放回画布上：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(10, 10, 50, 50);

function copy() {
  var imgData = ctx.getImageData(10, 10, 50, 50);
  ctx.putImageData(imgData, 10, 70);
}
</script>
<button onclick="copy()">Copy</button>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(10, 10, 50, 50);

function copy() {
  var imgData = ctx.getImageData(10, 10, 50, 50);
  ctx.putImageData(imgData, 10, 70);
}
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| putImageData() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`putImageData()` 方法将图像数据（来自指定的 `ImageData` 对象）放回画布上。

**提示：** 了解 [getImageData()](canvas_getimagedata.md) 方法，该方法复制画布上指定矩形的像素数据。

**提示：** 了解创建新的空白 `ImageData` 对象的 [createImageData()](canvas_createimagedata.md) 方法。

## JavaScript 语法

| JavaScript 语法: | *context*.putImageData(*imgData,x,y,**dirtyX,dirtyY,dirtyWidth,dirtyHeight*); |
| ---- | ---- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ---- | ---- |
| *imgData*     | 指定要放回画布上的 ImageData 对象 |
| *x*           | ImageData 对象左上角的 x 坐标（以像素为单位） |
| *y*           | ImageData 对象左上角的 y 坐标（以像素为单位） |
| *dirtyX*      | 选修的。 将图像放置在画布上的水平 (x) 值（以像素为单位） |
| *dirtyY*      | 选修的。 将图像放置在画布上的垂直 (y) 值（以像素为单位） |
| *dirtyWidth*  | 选修的。 用于在画布上绘制图像的宽度 |
| *dirtyHeight* | 选修的。 用于在画布上绘制图像的高度 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
