HTML canvas getImageData() 方法
===

## 示例

下面的代码使用 `getImageData()` 复制画布上指定矩形的像素数据，然后使用 [`putImageData()`](./canvas_putimagedata.md) 将图像数据放回画布上：

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
| ----- | --- | --- | --- | --- | --- |
| `getImageData()` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`getImageData()` 方法返回一个 `ImageData` 对象，该对象复制画布上指定矩形的像素数据。

**注意：** `ImageData` 对象不是图片，它指定画布上的一个部分（矩形），并保存该矩形内每个像素的信息。

对于 `ImageData` 对象中的每个像素，都有四个信息，即 RGBA 值：

R - 红色（0-255）\
G - 绿色（0-255）\
B - 蓝色（0-255）\
A - Alpha 通道（从 0-255；0 是透明的，255 是完全可见的）

`color/alpha` 信息保存在一个数组中，并存储在 `ImageData` 对象的 [data](canvas_imagedata_data.md) 属性中。

**提示：** 处理完数组中的 `color/alpha` 信息后，您可以使用 [putImageData()](canvas_putimagedata.md) 方法将图像数据复制回画布上。

**例子:**

获取返回的 ImageData 对象中第一个像素的 color/alpha 信息的代码：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<div>color/alpha 信息： <b id="info"></b></div>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(10, 10, 50, 50);

var imgData = ctx.getImageData(30, 30, 50, 50);
red = imgData.data[0];
green = imgData.data[1];
blue = imgData.data[2];
alpha = imgData.data[3];
// alert(red + " " + green + " " + blue + " " + alpha);
document.getElementById('info').innerHTML = red + " " + green + " " + blue + " " + alpha;
</script>
```

JavaScript:

```js
red=imgData.data[0];
green=imgData.data[1];
blue=imgData.data[2];
alpha=imgData.data[3];
```

**提示：** 您还可以使用 getImageData() 方法反转画布上图像的每个像素的颜色。

循环遍历所有像素并使用以下公式更改颜色值：

```js
red=255-old_red;
green=255-old_green;
blue=255-old_blue;
```

## JavaScript 语法

| JavaScript 语法: | *context*.getImageData(*x,y,width,height*); |
| ---- | ---- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ---- | ---- |
| *x*       | 开始复制的左上角的 x 坐标（以像素为单位） |
| *y*       | 开始复制的左上角的 y 坐标（以像素为单位） |
| *width*   | 您将复制的矩形区域的宽度 |
| *height*  | 您将复制的矩形区域的高度 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

使用 getImageData() 反转画布上图像的每个像素的颜色：

```html idoc:preview:iframe
<img id="scream" src="../assets/workplace.jpg" width="220" height="277">
<canvas id="myCanvas" width="220" height="277" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
document.getElementById("scream").onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 0, 0);
  var imgData = ctx.getImageData(0, 0, c.width, c.height);
  // 反转颜色
  var i;
  for (i = 0; i < imgData.data.length; i += 4) {
    imgData.data[i] = 255 - imgData.data[i];
    imgData.data[i+1] = 255 - imgData.data[i+1];
    imgData.data[i+2] = 255 - imgData.data[i+2];
    imgData.data[i+3] = 255;
  }
  ctx.putImageData(imgData, 0, 0);
};
</script>
```

JavaScript:

```js
document.getElementById("scream").onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 0, 0);
  var imgData = ctx.getImageData(0, 0, c.width, c.height);
  // 反转颜色
  var i;
  for (i = 0; i < imgData.data.length; i += 4) {
    imgData.data[i] = 255 - imgData.data[i];
    imgData.data[i+1] = 255 - imgData.data[i+1];
    imgData.data[i+2] = 255 - imgData.data[i+2];
    imgData.data[i+3] = 255;
  }
  ctx.putImageData(imgData, 0, 0);
};
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
