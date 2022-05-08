HTML canvas transform() 方法
===

## 示例

绘制一个矩形，使用 `transform()` 添加一个新的变换矩阵，再次绘制矩形，添加一个新的变换矩阵，然后再次绘制矩形。 请注意，每次调用 `transform()` 时，它都会建立在前面的转换矩阵之上：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.fillStyle = "yellow";
ctx.fillRect(0, 0, 250, 100)

ctx.transform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 250, 100);

ctx.transform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "blue";
ctx.fillRect(0, 0, 250, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.fillStyle = "yellow";
ctx.fillRect(0, 0, 250, 100)

ctx.transform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 250, 100);

ctx.transform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "blue";
ctx.fillRect(0, 0, 250, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| `transform()` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

画布上的每个对象都有一个当前变换矩阵。

`transform()` 方法替换了当前的变换矩阵。 它将当前变换矩阵与由下式描述的矩阵相乘：

|   |   |   |
| - | - | - |
| a | c | e |
| b | d | f |
| 0 | 0 | 1 |

换句话说，`transform()` 方法允许您缩放、旋转、移动和倾斜当前上下文。

**注意：** 转换只会影响调用 `transform()` 方法后的绘图。

**注意：** `transform()` 方法的行为与由 [rotate()](./canvas_rotate.md)、[scale()](./canvas_scale.md)、[translate()](./canvas_translate.md) 或 `transform()` 进行的其他转换相关。 示例：如果您已经将绘图设置为 2，并且 `transform()` 方法将您的绘图缩放了 2，那么您的绘图现在将缩放 4。

**提示：** 查看 [setTransform()](canvas_settransform.md) 方法，它的行为与其他转换不同。

| JavaScript 语法: | *context*.transform(*a,b,c,d,e,f*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *a* | 水平缩放 |
| *b* | 水平倾斜 |
| *c* | 垂直倾斜 |
| *d* | 垂直缩放 |
| *e* | 水平移动 |
| *f* | 垂直移动 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg