HTML canvas textAlign 方法
===

## 示例

在位置 150 创建一条红线。位置 150 是下例中定义的所有文本的锚点。 研究每个 `textAlign` 属性值的效果：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="200" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 在位置 150 创建一条红线
ctx.strokeStyle = "red";
ctx.moveTo(150, 20);
ctx.lineTo(150, 170);
ctx.stroke();

ctx.font = "15px Arial";    

// 显示不同的 textAlign 值
ctx.textAlign = "start";      
ctx.fillText("textAlign=start", 150, 60);        
ctx.textAlign = "end";      
ctx.fillText("textAlign=end", 150, 80);                  
ctx.textAlign = "left";      
ctx.fillText("textAlign=left", 150, 100);
ctx.textAlign = "center";     
ctx.fillText("textAlign=center",150, 120);              
ctx.textAlign = "right";      
ctx.fillText("textAlign=right",150, 140);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
// 在位置 150 创建一条红线
ctx.strokeStyle = "red";
ctx.moveTo(150, 20);
ctx.lineTo(150, 170);
ctx.stroke();
ctx.font = "15px Arial";
// 显示不同的 textAlign 值
ctx.textAlign = "start";
ctx.fillText("textAlign=start", 150, 60);
ctx.textAlign = "end";
ctx.fillText("textAlign=end", 150, 80);
ctx.textAlign = "left";
ctx.fillText("textAlign=left", 150, 100);
ctx.textAlign = "center";
ctx.fillText("textAlign=center", 150, 120);
ctx.textAlign = "right";
ctx.fillText("textAlign=right", 150, 140);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| textAlign | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`textAlign` 属性根据锚点设置或返回文本内容的当前对齐方式。

通常，文本将在指定的位置 **START**，但是，如果您设置 `textAlign="right"` 并将文本放置在位置 150，这意味着文本应该在位置 150 **END**。

**提示：** 使用 [fillText()](canvas_filltext.md) 或 [strokeText()](canvas_stroketext.md) 方法在画布上实际绘制和定位文本。

| 默认值: | `start` |
| ----- | ----- |
| JavaScript 语法: | *context*.textAlign="center/end/left/right/start"; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| start  | 默认。 文本从指定位置开始 |
| end    | 文本在指定位置结束 |
| center | 文本的中心放置在指定位置 |
| left   | 文本从指定位置开始 |
| right  | 文本在指定位置结束 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg