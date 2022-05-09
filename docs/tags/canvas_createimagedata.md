HTML canvas createImageData() 方法
===

## 示例

创建一个 `100*100` 像素的 `ImageData` 对象，其中每个像素都是红色的，并将其放到画布上：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var imgData = ctx.createImageData(100, 100);

var i;
for (i = 0; i < imgData.data.length; i += 4) {
  imgData.data[i+0] = 255;
  imgData.data[i+1] = 0;
  imgData.data[i+2] = 0;
  imgData.data[i+3] = 255;
}
ctx.putImageData(imgData, 10, 10);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var imgData = ctx.createImageData(100, 100);

var i;
for (i = 0; i < imgData.data.length; i += 4) {
  imgData.data[i+0] = 255;
  imgData.data[i+1] = 0;
  imgData.data[i+2] = 0;
  imgData.data[i+3] = 255;
}
ctx.putImageData(imgData, 10, 10);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| createImageData() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`createImageData()` 方法创建一个新的空白 `ImageData` 对象。新对象的像素值默认为透明黑色。

对于 `ImageData` 对象中的每个像素，都有四个信息，即 RGBA 值：

R - 红色（0-255）\
G - 绿色（0-255）\
B - 蓝色（0-255）\
A - Alpha 通道（从 0-255；0 是透明的，255 是完全可见的）

因此，透明黑色表示：(0,0,0,0)。

color/alpha 信息保存在一个数组中，由于该数组包含每个像素的 4 条信息，因此该数组的大小是 `ImageData` 对象大小的 4 倍：width\*height\*4。 （查找数组大小的更简单方法是使用 ImageDataObject.data.length）

包含 color/alpha 信息的数组存储在 `ImageData` 对象的 [data](canvas_imagedata_data.md) 属性中。

**提示：** 处理完数组中的颜色/alpha 信息后，您可以使用 [putImageData()](canvas_putimagedata.md) 方法将图像数据复制回画布上。

**例子:**

使 `ImageData` 对象中的第一个像素变为红色的语法：

```js
imgData=ctx.createImageData(100,100);

imgData.data[0]=255;
imgData.data[1]=0;
imgData.data[2]=0;
imgData.data[3]=255;
```

使 `ImageData` 对象中的第二个像素变为绿色的语法：

```js
imgData=ctx.createImageData(100,100);

imgData.data[4]=0;
imgData.data[5]=255;
imgData.data[6]=0;
imgData.data[7]=255;
```

## JavaScript 语法

`createImageData()` 方法有两个版本：

1. 这将创建一个具有指定尺寸（以像素为单位）的新 ImageData 对象：

| JavaScript 语法: | var imgData=*context*.createImageData(*width,height*); |
| ---- | ---- |
<!--rehype:style=width: 100%; display: inline-table;-->

2. 这将创建一个与 anotherImageData 指定的对象具有相同尺寸的新 ImageData 对象（这不会复制图像数据）：

| JavaScript 语法: | var imgData=*context*.createImageData(*imageData*); |
| ---- | ---- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ---- | ---- |
| *width*     | 新 `ImageData` 对象的宽度，以像素为单位 |
| *height*    | 新 `ImageData` 对象的高度，以像素为单位 |
| *imageData* | 另一个 `ImageData` 对象 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
