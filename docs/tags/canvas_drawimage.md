HTML canvas drawImage() 方法
===

## 示例

![The Scream](../assets/chrome.svg)

将图像绘制到画布上：

```html idoc:preview:iframe
<div>要使用的图像：</div>
<img id="scream" width="65" height="65" src="../assets/chrome.svg">
<div>Canvas:</div>
<canvas id="myCanvas" width="240" height="297" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。 </canvas>

<script>
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 10, 10);
}
</script>
```

JavaScript:

```js
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 10, 10);
};
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| drawImage() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`drawImage()` 方法在画布上绘制图像、画布或视频。

`drawImage()` 方法还可以绘制图像的一部分，和/或增加/减小图像大小。

**注意：** 您不能在图像加载之前调用 `drawImage()` 方法。 为确保图像已加载，您可以从 `window.onload()` 或 `document.getElementById("imageID").onload` 调用 `drawImage()`。

## JavaScript 语法

将图像放置在画布上：

| JavaScript 语法: | *context*.drawImage(*img,x,y*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

将图像放置在画布上，并指定图像的宽度和高度：

| JavaScript 语法: | *context*.drawImage(*img,x,y,width,height*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

裁剪图像并将裁剪的部分放置在画布上：

| JavaScript 语法: | *context*.drawImage(*img,sx,sy,swidth,sheight,x,y,width,height*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *img*     | 指定要使用的图像、画布或视频元素 |
| *sx*      | 选修的。 开始剪辑的 x 坐标 |
| *sy*      | 选修的。 y 坐标从哪里开始剪辑 |
| *swidth*  | 选修的。 剪切图像的宽度 |
| *sheight* | 选修的。 剪切图像的高度 |
| *x*       | 将图像放置在画布上的 x 坐标 |
| *y*       | y 坐标在画布上放置图像的位置 |
| *width*   | 选修的。 要使用的图像宽度（拉伸或缩小图像） |
| *height*  | 选修的。 要使用的图像高度（拉伸或缩小图像） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

将图像放置在画布上，并指定图像的宽度和高度：

```html idoc:preview:iframe
<div>要使用的图像：</div>
<img id="scream" width="120" height="120" src="../assets/chrome.svg" alt="The Scream">

<div>Canvas:</div>
<canvas id="myCanvas" width="240" height="297" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。 </canvas>

<script>
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 10, 10, 150, 180);
}
</script>
```

JavaScript:

```js
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 10, 10, 150, 180);
};
```

裁剪图像并将裁剪的部分放置在画布上

```html idoc:preview:iframe
<div>要使用的图像：</div>
<img id="scream" src="../assets/workplace.jpg" alt="The Scream" width="120" height="120">

<div>Canvas:</div>
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。 </canvas>

<script>
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 90, 130, 50, 60, 10, 10, 50, 60);
};
</script>
```

JavaScript:

```js
window.onload = function() {
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  ctx.drawImage(img, 90, 130, 50, 60, 10, 10, 50, 60);
};
```

要使用的视频（按播放开始演示）：

[](../assets/mov_bbb.mp4)

Canvas:

```html idoc:preview:iframe
<p>使用视频：</p>
<video id="video1" controls width="270" autoplay>
  <source src="../assets/mov_bbb.mp4" type='video/mp4'>
</video>

<p>要使用的视频（按播放开始演示）：</p>
<canvas id="myCanvas" width="270" height="135" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var v = document.getElementById("video1");
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var i;

v.addEventListener("play", function() {i = window.setInterval(function() {ctx.drawImage(v,5,5,260,125)},20);}, false);
v.addEventListener("pause", function() {window.clearInterval(i);}, false);
v.addEventListener("ended", function() {clearInterval(i);}, false); 
</script>
```

JavaScript（代码每 20 毫秒绘制一次视频的当前帧）：

```js
var v = document.getElementById("video1");
var c = document.getElementById("myCanvas");
var ctx = c.getContext('2d');
var i;

v.addEventListener('play',function() {i=window.setInterval(function() {ctx.drawImage(v,5,5,260,125)},20);},false);
v.addEventListener('pause',function() {window.clearInterval(i);},false);
v.addEventListener('ended',function() {clearInterval(i);},false);
```



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
