HTML canvas setTransform() 方法
===

## 示例

绘制一个矩形，使用 `setTransform()` 重置并创建一个新的变换矩阵，再次绘制矩形，重置并创建一个新的变换矩阵，然后再次绘制矩形。 请注意，每次调用 `setTransform()` 时，它都会重置之前的变换矩阵，然后构建新矩阵，因此在下面的示例中，红色矩形没有显示，因为它位于蓝色矩形下方：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.fillStyle = "yellow";
ctx.fillRect(0, 0, 250, 100)

ctx.setTransform(1,0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 250, 100);

ctx.setTransform(1,0.5, -0.5, 1, 30, 10);
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

ctx.setTransform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "red";
ctx.fillRect(0, 0, 250, 100);

ctx.setTransform(1, 0.5, -0.5, 1, 30, 10);
ctx.fillStyle = "blue";
ctx.fillRect(0, 0, 250, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| setTransform() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

画布上的每个对象都有一个当前变换矩阵。

`setTransform()` 方法将当前变换重置为单位矩阵，然后使用相同的参数运行 [transform()](canvas_transform.md)。

换句话说，`setTransform()` 方法允许您缩放、旋转、移动和倾斜当前上下文。

**注意：** 转换只会影响调用 `setTransform` 方法后的绘图。

| JavaScript 语法: | *context*.setTransform(*a,b,c,d,e,f*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *a*       | 水平缩放 |
| *b*       | 水平倾斜 |
| *c*       | 垂直倾斜 |
| *d*       | 垂直缩放 |
| *e*       | 水平移动 |
| *f*       | 垂直移动 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg