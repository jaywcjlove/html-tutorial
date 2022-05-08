HTML canvas fillStyle 属性
===

## 示例

为矩形定义红色填充颜色：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "#FF0000";
  ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "#FF0000";
ctx.fillRect(20, 20, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| fillStyle() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`fillStyle` 属性设置或返回用于填充绘图的颜色、渐变或图案。

| 默认值: | `#000000` |
| ------- | ------- |
| JavaScript 语法: | *context*.fillStyle=`color`\|`gradient`\|`pattern`; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *color*    | 一个 [CSS 颜色值](../reference/colornames.md)，指示绘图的填充颜色。 默认值为 `#000000` |
| *gradient* | 用于填充绘图的渐变对象（[linear](canvas_createlineargradient.md) 或 [radial](canvas_createradialgradient.md)） |
| *pattern*  | 用于填充绘图的 [pattern](canvas_createpattern.md) 对象 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg