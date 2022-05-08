HTML canvas scale() 方法
===

## 示例

绘制一个矩形，缩放到 200%，然后再次绘制矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.strokeRect(5, 5, 25, 15);
ctx.scale(2, 2);
ctx.strokeRect(5, 5, 25, 15);
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.strokeRect(5, 5, 25, 15);
ctx.scale(2, 2);
ctx.strokeRect(5, 5, 25, 15);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| `scale()` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`scale()` 方法缩放当前图形，更大或更小。

**注意：** 如果您缩放图纸，所有未来的图纸也将被缩放。 定位也将被缩放。 如果你缩放 `(2,2）`； 绘图将放置在您指定的距离画布左侧和顶部两倍的位置。

| JavaScript 语法: | *context*.scale(*scalewidth,scaleheight*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *scalewidth*  | 缩放当前图形的宽度（1=100%、0.5=50%、2=200% 等） |
| *scaleheight* | 缩放当前图形的高度（1=100%、0.5=50%、2=200% 等） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

绘制一个矩形，缩放到 200%，再次绘制矩形，缩放到 200%，再次绘制矩形，缩放到 200%，再次绘制矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="170" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.strokeRect(5, 5, 25, 15);
  ctx.scale(2, 2);
  ctx.strokeRect(5, 5, 25, 15);
  ctx.scale(2, 2);
  ctx.strokeRect(5, 5, 25, 15);
  ctx.scale(2, 2);
  ctx.strokeRect(5, 5, 25, 15);
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.strokeRect(5, 5, 25, 15);
ctx.scale(2, 2);
ctx.strokeRect(5, 5, 25, 15);
ctx.scale(2, 2);
ctx.strokeRect(5, 5, 25, 15);
ctx.scale(2, 2);
ctx.strokeRect(5, 5, 25, 15);
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg