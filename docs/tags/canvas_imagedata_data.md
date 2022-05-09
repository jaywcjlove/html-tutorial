HTML canvas ImageData data 属性
===

## 示例

创建一个 100\*100 像素的 ImageData 对象，其中每个像素都设置为红色：

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
  imgData.data[i + 0] = 255;
  imgData.data[i + 1] = 0;
  imgData.data[i + 2] = 0;
  imgData.data[i + 3] = 255;
}
ctx.putImageData(imgData, 10, 10);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| data     | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`data` 属性返回一个包含指定 `ImageData` 对象的图像数据的对象。

对于 `ImageData` 对象中的每个像素，都有四个信息，即 RGBA 值：

R - 红色（0-255）\
G - 绿色（0-255）\
B - 蓝色（0-255）\
A - Alpha 通道（从 0-255；0 是透明的，255 是完全可见的）

color/alpha 信息保存在一个数组中，并存储在 `ImageData` 对象的 data 属性中。

**例子:**

使 `ImageData` 对象中的第一个像素变为红色的语法：

```js
imgData=ctx.createImageData(100, 100);

imgData.data[0] = 255;
imgData.data[1] = 0;
imgData.data[2] = 0;
imgData.data[3] = 255;
```

使 ImageData 对象中的第二个像素变为绿色的语法：

```js
imgData = ctx.createImageData(100, 100);

imgData.data[4] = 0;
imgData.data[5] = 255;
imgData.data[6] = 0;
imgData.data[7] = 255;
```

**提示：** 查看 [createImageData()](canvas_createimagedata.md)、[getImageData()](canvas_getimagedata.md) 和 [putImageData()](canvas_putimagedata.md) 以了解有关 ImageData 对象的更多信息。
## JavaScript 语法

| JavaScript 语法: | *imageData*.data; |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
