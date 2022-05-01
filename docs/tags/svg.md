HTML \<svg> Tag
===

## 示例

画一个圆圈：

```html idoc:preview:iframe
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```
<!--rehype:style=height: 130px;-->

## 定义和用法

`<svg>` 标签定义了 SVG 图形的容器。

SVG 有多种绘制路径、框、圆、文本和图形图像的方法。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<svg>  | 4.0 | 9.0 | 3.0 | 3.2 | 10.1 |

## 更多示例

画一个矩形：

```html idoc:preview:iframe
<svg width="400" height="100">
  <rect width="400" height="100" style="fill:rgb(0,0,255);stroke-width:10;stroke:rgb(0,0,0)" />
</svg>
```
<!--rehype:style=height: 130px;-->

画一个圆角的正方形：

```html idoc:preview:iframe
<svg width="400" height="180">
  <rect
    x="50" y="20" rx="20" ry="20"
    width="150"
    height="150"
    style="fill:red;stroke:black;stroke-width:5;opacity:0.5"
  />
</svg>
```

画一颗星：

```html idoc:preview:iframe
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
```
<!--rehype:style=height: 230px;-->

绘制一个 SVG 标志：

```html idoc:preview:iframe
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
</svg>
```

## 相关页面

HTML 教程: [HTML SVG](../tutorial/svg.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg