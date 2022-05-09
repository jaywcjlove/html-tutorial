HTML canvas globalCompositeOperation 属性
===

## 示例

使用两个不同的 `globalCompositeOperation` 值绘制矩形。 红色矩形是目标图像。 蓝色矩形是源图像：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "red";
  ctx.fillRect(20, 20, 75, 50);
  ctx.fillStyle = "blue";
  ctx.globalCompositeOperation = "source-over";
  ctx.fillRect(50, 50, 75, 50);
  ctx.fillStyle = "red";
  ctx.fillRect(150, 20, 75, 50);
  ctx.fillStyle = "blue";
  ctx.globalCompositeOperation = "destination-over";
  ctx.fillRect(180, 50, 75, 50);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.fillStyle = "red";
ctx.fillRect(20, 20, 75, 50);
ctx.globalCompositeOperation = "source-over";
ctx.fillStyle = "blue";
ctx.fillRect(50, 50, 75, 50);

ctx.fillStyle = "red";
ctx.fillRect(150, 20, 75, 50);
ctx.globalCompositeOperation = "destination-over";
ctx.fillStyle = "blue";
ctx.fillRect(180, 50, 75, 50);
```

## 浏览器支持

![chrome][1] ![edge][2] ![firefox][3] ![safari][4] ![opera][5]

Internet Explorer 9、Firefox、Opera、Chrome 和 Safari 支持 globalCompositeOperation 属性。

## 定义和用法

`globalCompositeOperation` 属性设置或返回如何将源（新）图像绘制到目标（现有）图像上。

*源图像 =* 您将要放置到画布上的绘图。

*目标图像 =* 已经放置在画布上的绘图。

| 默认值: | `source-over` |
| ------ | ------ |
| JavaScript syntax: | *context*.globalCompositeOperation="source-in"; |

## 属性值

| 值 Value  | 描述 Description |
| ------ | ------ |
| source-over      | 默认。在 **目标图像** 上显示 **源图像** | 
| source-atop      | 在 **目标图像** 顶部显示 **源图像**。 **目标图像**之外的**源图像**部分未显示 | 
| source-in        | 将 **源图像** 显示到 **目标图像**。仅显示**目标图像**内部的**源图像**部分，并且**目标图像**是透明的 | 
| source-out       | 显示**目标图像**之外的**源图像**。仅显示**目标图像**之外的**源图像**部分，并且**目标图像**是透明的 | 
| destination-over | 在**源图像**上显示**目标图像** | 
| destination-atop | 在**源图像**之上显示**目标图像**。未显示 **源图像** 之外的 **目标图像** 部分 | 
| destination-in   | 在**源图像**中显示**目标图像**。仅显示**源图像**内部的**目标图像**部分，并且**源图像**是透明的 | 
| destination-out  | 显示**源图像**中的**目标图像**。仅显示 **目标图像** 在 **源图像** 之外的部分，并且 **源图像** 是透明的 | 
| lighter          | 显示**源图像**+**目标图像** | 
| copy             | 显示**源图像**。**目标图像**被忽略 | 
| xor              | **源图像**与**目标图像**使用异或组合 | 



## 更多示例

所有 globalCompositeOperation 属性值：

```html idoc:preview:iframe
<style>
canvas {
  border: 1px solid #d3d3d3;
  margin-right: 10px;
  margin-bottom: 20px;
}
</style>
<script>
var gco = new Array();
gco.push("source-atop");
gco.push("source-in");
gco.push("source-out");
gco.push("source-over");
gco.push("destination-atop");
gco.push("destination-in");
gco.push("destination-out");
gco.push("destination-over");
gco.push("lighter");
gco.push("copy");
gco.push("xor");

var n;
for (n = 0; n < gco.length; n++) {
  document.write("<div id='p_" + n + "' style='float:left;'>" + gco[n] + ":<br>");
  var c = document.createElement("canvas");
  c.width = 120;
  c.height = 100;
  document.getElementById("p_" + n).appendChild(c);
  var ctx = c.getContext("2d");    
  ctx.fillStyle = "blue";
  ctx.fillRect(10, 10, 50, 50);
  ctx.globalCompositeOperation = gco[n];
  ctx.beginPath();
  ctx.fillStyle = "red";
  ctx.arc(50, 50, 30, 0, 2 * Math.PI);
  ctx.fill();
  document.write("</div>");
}
</script>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
