HTML SVG Graphics
===

SVG 以 XML 格式定义基于矢量的图形。

## 什么是 SVG？

* SVG 代表可缩放矢量图形
* SVG 用于为 Web 定义图形
* SVG 是 W3C 推荐的

## HTML \<svg> 元素

HTML [`<svg>`](../tags/svg.md) 元素是 SVG 图形的容器。

SVG 有多种绘制路径、框、圆、文本和图形图像的方法。

## 浏览器支持

表中的数字指定了第一个完全支持 [`<svg>`](../tags/svg.md) 元素的浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| \<svg>  | 4.0 | 9.0 | 3.0 | 3.2 | 10.1 |

## SVG 圆

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body>
  <svg width="100" height="100">
    <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow">
  </svg>
</body>
</html>
```
<!--rehype:style=height: 150px;-->

## SVG 矩形

```html idoc:preview:iframe
<svg width="400" height="100">
  <rect width="400" height="100" style="fill:rgb(0,0,255); stroke-width:10; stroke:rgb(0,0,0)" />
</svg>
```
<!--rehype:style=height: 130px;-->

## SVG 圆角矩形

```html idoc:preview
<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
</svg>
```
<!--rehype:style=height: 230px;-->

## SVG 星

```html idoc:preview
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
```
<!--rehype:style=height: 230px;-->

## SVG Logo

```html idoc:preview
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
  Sorry, your browser does not support inline SVG.
</svg>
```
<!--rehype:style=height: 180px;-->

## SVG 和 Canvas 的区别

SVG 是一种用 XML 描述 2D 图形的语言。

Canvas 动态绘制 2D 图形（使用 JavaScript）。

SVG 是基于 XML 的，这意味着每个元素都可以在 SVG DOM 中使用。 您可以为元素附加 JavaScript 事件处理程序。

在 SVG 中，每个绘制的形状都被记忆为一个对象。 如果 SVG 对象的属性发生变化，浏览器可以自动重新渲染形状。

画布是逐像素渲染的。 在画布中，一旦图形被绘制出来，浏览器就会忘记它。 如果要更改其位置，则需要重新绘制整个场景，包括可能已被图形覆盖的任何对象。

## Canvas 和 SVG 的比较

The table below shows some important differences between Canvas and SVG:

| Canvas | SVG |
| ---- | ---- |
| * 取决于分辨率 <br />* 不支持事件处理程序 <br />* 文本渲染能力差 <br />* 您可以将生成的图像保存为 .png 或 .jpg <br />* 非常适合图形密集型游戏 | * 独立于分辨率 <br />* 支持事件处理程序 <br />* 最适合具有大渲染区域的应用程序（谷歌地图）<br />* 如果复杂，渲染速度会很慢（任何使用 DOM 的东西都会很慢）<br /> * 不适合游戏应用 |



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
