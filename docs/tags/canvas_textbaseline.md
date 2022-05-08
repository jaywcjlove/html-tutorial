HTML canvas textBaseline 属性
===

## 示例

在 `y=100` 处画一条红线，然后用不同的 `textBaseline` 值将每个单词放在 `y=100` 处：

```html idoc:preview:iframe
<canvas id="myCanvas" width="400" height="200" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 在 y=100 处画一条红线
ctx.strokeStyle = "red";
ctx.moveTo(5, 100);
ctx.lineTo(395, 100);
ctx.stroke();

ctx.font = "20px Arial"
// 将每个单词放在 y=100 处，并使用不同的 textBaseline 值
ctx.textBaseline = "top"; 
ctx.fillText("Top", 5, 100); 
ctx.textBaseline = "bottom"; 
ctx.fillText("Bottom", 50, 100); 
ctx.textBaseline = "middle"; 
ctx.fillText("Middle", 120, 100); 
ctx.textBaseline = "alphabetic"; 
ctx.fillText("Alphabetic", 190, 100); 
ctx.textBaseline = "hanging"; 
ctx.fillText("Hanging", 290, 100); 
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 在 y=100 处画一条红线
ctx.strokeStyle = "red";
ctx.moveTo(5, 100);
ctx.lineTo(395, 100);
ctx.stroke();

ctx.font = "20px Arial"
// 将每个单词放在 y=100 处，并使用不同的 textBaseline 值
ctx.textBaseline = "top"; 
ctx.fillText("Top", 5, 100); 
ctx.textBaseline = "bottom"; 
ctx.fillText("Bottom", 50, 100); 
ctx.textBaseline = "middle"; 
ctx.fillText("Middle", 120, 100); 
ctx.textBaseline = "alphabetic"; 
ctx.fillText("Alphabetic", 190, 100); 
ctx.textBaseline = "hanging"; 
ctx.fillText("Hanging", 290, 100); 
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| textBaseline | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** `textBaseline` 属性在不同浏览器中的工作方式不同，尤其是在使用 `hanging` 或 `ideographic` 时。

## 定义和用法

`textBaseline` 属性设置或返回绘制文本时使用的当前文本基线。

下图演示了 `textBaseline` 属性支持的各种基线：

![textBaseline 插图](../assets/img_textbaseline.gif)

**注意：** [fillText()](canvas_filltext.md) 和 [strokeText()](canvas_stroketext.md) 方法将在画布上定位文本时使用指定的 textBaseline 值。

| 默认值:     | `alphabetic` |
| ------- | ------- |
| JavaScript 语法: | *context*.textBaseline="alphabetic/top/hanging/middle/ideographic/bottom"; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| alphabetic  | 默认。 文本基线是正常的字母基线  |
| top         | 文本基线是 em 正方形的顶部  |
| hanging     | 文字基线是悬挂基线  |
| middle      | 文本基线是 em 正方形的中间  |
| ideographic | 文本基线是表意基线  |
| bottom      | 文本基线是边界框的底部  |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg