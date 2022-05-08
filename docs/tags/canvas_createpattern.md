HTML `<canvas>` createPattern() 方法
===

## 示例

![chrome](../assets/chrome.svg)

水平和垂直重复图像：

```html idoc:preview:iframe
<p>要使用的图像：</p>
<img src="../assets/chrome.svg" id="lamp" width="32" height="32">
<p>Canvas:</p>
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>
<br>
<button onclick="draw('repeat')">Repeat</button> 
<button onclick="draw('repeat-x')">Repeat-x</button> 
<button onclick="draw('repeat-y')">Repeat-y</button> 
<button onclick="draw('no-repeat')">No-repeat</button>
<script>
  function draw(direction) {
    var c = document.getElementById("myCanvas");
    var ctx = c.getContext("2d");
    ctx.clearRect(0, 0, c.width, c.height); 
    var img = document.getElementById("lamp")
    var pat = ctx.createPattern(img, direction);
    ctx.rect(0, 0, 150, 100);
    ctx.fillStyle = pat;
    ctx.fill();
  }
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var img = document.getElementById("lamp");
var pat = ctx.createPattern(img, "repeat");
ctx.rect(0, 0, 150, 100);
ctx.fillStyle = pat;
ctx.fill();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| createPattern() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`createPattern()` 方法在指定方向重复指定元素。

该元素可以是图像、视频或另一个 \<canvas> 元素。

重复元素可用于绘制/填充矩形、圆形、线条等。

| JavaScript 语法: | *context*.createPattern(*image*,"repeat\|repeat-x\|repeat-y\|no-repeat"); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *image*   | 指定要使用的图案的图像、画布或视频元素 |
| repeat    | 默认。 图案水平和垂直重复 |
| repeat-x  | 图案仅水平重复 |
| repeat-y  | 图案仅垂直重复 |
| no-repeat | 花样只显示一次（不重复） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg