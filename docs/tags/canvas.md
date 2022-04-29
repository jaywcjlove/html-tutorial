HTML \<canvas> Tag
===

用于通过脚本（通常是 JavaScript）动态绘制图形。

## 示例

即时绘制一个红色矩形，并将其显示在 \<canvas> 元素中：

```html idoc:preview:iframe
<canvas id="myCanvas">
  Your browser does not support the canvas tag.
</canvas>
<script>
  var canvas = document.getElementById("myCanvas");
  var ctx = canvas.getContext("2d");
  ctx.fillStyle = "#FF0000";
  ctx.fillRect(0, 0, 80, 80);
</script>
```

## 定义和用法

`<canvas>` 标签用于通过脚本（通常是 JavaScript）动态绘制图形。

`<canvas>` 标签是透明的，只是图形的容器，你必须使用脚本来实际绘制图形。

`<canvas>` 元素内的任何文本都将显示在禁用 JavaScript 的浏览器和不支持 `<canvas>` 的浏览器中。

## 提示和注意事项

**提示：** 有关所有属性和方法的完整参考，请访问我们的 [HTML Canvas 参考](../reference/canvas.md)。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<canvas> | 4.0 | 9.0 | 2.0 | 3.1 | 9.0 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [height](./canvas_height.md) | *pixels* | 指定画布的高度。 默认值为 150 |
| [width](./canvas_width.md)   | *pixels* | 指定画布的宽度 默认值为 300 |

## 全局属性

`<button>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<button>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

另一个 \<canvas> 示例：

```html idoc:preview:iframe
<canvas id="myCanvas"> 您的浏览器不支持 canvas 标签。 </canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "red";
  ctx.fillRect(20, 20, 75, 50);
  //Turn transparency on
  ctx.globalAlpha = 0.2;
  ctx.fillStyle = "blue";
  ctx.fillRect(50, 50, 75, 50);
  ctx.fillStyle = "green";
  ctx.fillRect(80, 80, 75, 50);
</script>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<canvas>` 元素：

```css
canvas {
  height: 150px;
  width: 300px;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg