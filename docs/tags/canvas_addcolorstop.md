HTML canvas addColorStop() 方法
===

## 示例

定义一个从黑色到白色的渐变，作为矩形的填充样式：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");

  var grd = ctx.createLinearGradient(0, 0, 170, 0);
  grd.addColorStop(0, "black");
  grd.addColorStop(1, "white");

  ctx.fillStyle = grd;
  ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById('myCanvas');
var ctx = c.getContext('2d');

var grd = ctx.createLinearGradient(0, 0, 170, 0);
grd.addColorStop(0, "black");
grd.addColorStop(1, "white");

ctx.fillStyle = grd;
ctx.fillRect(20, 20, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| addColorStop() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`addColorStop()` 方法指定渐变对象中的颜色和位置。

`addColorStop()` 方法与 [createLinearGradient()](canvas_createlineargradient.md) 或 [createRadialGradient()](canvas_createradialgradient.md) 一起使用。

**注意：** 您可以多次调用 addColorStop() 方法来更改渐变。 如果您对渐变对象省略此方法，渐变将不可见。 您需要至少创建一个色标才能获得可见的渐变。

| JavaScript 语法: | *gradient*.addColorStop(*stop*,*color*); |
| ------ | ------ |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *stop*    | 一个介于 0.0 和 1.0 之间的值，表示渐变中开始和结束之间的位置 |
| *color*   | 在 *stop* 位置显示的 [CSS 颜色值](../reference/colornames.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

使用多个 addColorStop() 方法定义渐变：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
 
var grd = ctx.createLinearGradient(0, 0, 170, 0);
grd.addColorStop(0, "black");
grd.addColorStop("0.3", "magenta");
grd.addColorStop("0.5", "blue");
grd.addColorStop("0.6", "green");
grd.addColorStop("0.8", "yellow");
grd.addColorStop(1, "red");
 
ctx.fillStyle = grd;
ctx.fillRect(20, 20, 150, 100); 
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var grd = ctx.createLinearGradient(0, 0, 170, 0);
grd.addColorStop(0, "black");
grd.addColorStop("0.3", "magenta");
grd.addColorStop("0.5", "blue");
grd.addColorStop("0.6", "green");
grd.addColorStop("0.8", "yellow");
grd.addColorStop(1, "red");

ctx.fillStyle = grd;
ctx.fillRect(20, 20, 150, 100);
```



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg