HTML canvas strokeStyle 属性
===

## 示例

画一个矩形。 使用红色笔触颜色：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.strokeStyle = "#FF0000";
ctx.strokeRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.strokeStyle = "#FF0000";
ctx.strokeRect(20, 20, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| strokeStyle | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`strokeStyle` 属性设置或返回用于笔触的颜色、渐变或图案。

| 默认值: | `#000000` |
| ------- | ------- |
| JavaScript 语法: | *context*.strokeStyle=`color`\|`gradient`\|`pattern`; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *color*    | 一个 [CSS 颜色值](../reference/colornames.md)，表示绘图的笔触颜色。 默认值为 `#000000` |
| *gradient* | 用于创建渐变描边的渐变对象（[linear](canvas_createlineargradient.md) 或 [radial](canvas_createradialgradient.md)） |
| *pattern*  | 用于创建图案描边的 [pattern](canvas_createpattern.md) 对象 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

画一个矩形。 使用渐变笔触：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var gradient = ctx.createLinearGradient(0, 0, 170, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5", "blue");
gradient.addColorStop("1.0", "red");

// 填充渐变
ctx.strokeStyle = gradient;
ctx.lineWidth = 5;
ctx.strokeRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var gradient = ctx.createLinearGradient(0, 0, 170, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5" ,"blue");
gradient.addColorStop("1.0", "red");

// 填充渐变
ctx.strokeStyle = gradient;
ctx.lineWidth = 5;
ctx.strokeRect(20, 20, 150, 100);
```

用渐变笔划写下文本 `HTML Tutorial!`：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.font = "30px Verdana";

// 创建渐变
var gradient = ctx.createLinearGradient(0, 0, c.width, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5", "blue");
gradient.addColorStop("1.0", "red");

// 填充渐变
ctx.strokeStyle = gradient;
ctx.strokeText("HTML Tutorial!", 10, 50);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Verdana";
// 创建渐变
var gradient = ctx.createLinearGradient(0, 0, c.width, 0);
gradient.addColorStop("0", "magenta");
gradient.addColorStop("0.5", "blue");
gradient.addColorStop("1.0", "red");
// 填充渐变
ctx.strokeStyle = gradient;
ctx.strokeText("Big smile!", 10, 50);
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg