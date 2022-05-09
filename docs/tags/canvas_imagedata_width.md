HTML canvas ImageData width 属性
===

## 示例

提醒 ImageData 对象的宽度：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<div>imgData 的宽度为： <span id="info"></span></div>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var imgData = ctx.createImageData(100, 100);
document.getElementById('info').innerHTML = imgData.width;

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
document.getElementById('info').innerHTML = imgData.width
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| width    | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

该属性返回 ImageData 对象的宽度，以像素为单位。

**提示：** 查看 [createImageData()](canvas_createimagedata.md)、[getImageData()](canvas_getimagedata.md) 和 [putImageData()](canvas_putimagedata.md) 以了解有关 ImageData 对象的更多信息。

## JavaScript 语法

| JavaScript 语法: | *imgData*.width; |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg