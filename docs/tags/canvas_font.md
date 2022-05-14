HTML canvas font 属性
===

## 示例

在画布上写一个 `30px` 高的文本，使用字体“Arial”：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| font     | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`font` 属性设置或返回画布上文本内容的当前字体属性。

| 默认值: | `10px sans-serif` |
| ----- | ----- |
| JavaScript 语法: | *context*.font="italic small-caps bold 12px arial"; |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *font-style* | 指定字体样式。 可能的值：<br>* `normal` <br>* `italic` <br>* `oblique` | 
| *font-variant* | 指定字体变体。 可能的值：<br>* `normal` <br>* `small-caps` | 
| *font-weight* | 指定字体粗细。 可能的值：<br>* `normal` <br>* `bold` <br>* `bolder` <br>* `lighter` <br>* `100` <br>* `200` <br>* `300` <br>* `400` <br>* `500` <br>* `600` <br>* `700` <br>* `800` <br>* `900` | 
| *font-size/line-height* | 指定字体大小和行高，以像素为单位 | 
| *font-family*           | 指定字体系列 | 
| caption                 | 使用字体标题控件（如按钮、下拉菜单等） | 
| icon                    | 使用用于标签图标的字体 | 
| menu                    | 使用菜单中使用的字体（下拉菜单和菜单列表） | 
| message-box             | 使用对话框中使用的字体 | 
| small-caption           | 使用用于标签小控件的字体 | 
| status-bar              | 使用窗口状态栏中使用的字体 | 
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg