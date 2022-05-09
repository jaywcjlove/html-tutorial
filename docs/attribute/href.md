HTML href 属性
===

## 定义和用法

对于 [\<a>](../tags/a.md) 和 [\<area>](../tags/area.md) 元素，`href` 属性指定链接指向的页面的 URL。

对于 [\<base>](../tags/base.md) 元素，`href` 属性指定页面上所有相对 URL 的基本 URL。

对于 [\<link>](../tags/link.md) 元素，`href` 属性指定外部资源（通常是样式表文件）的位置（URL）。

## 适用于

`href` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<a>](../tags/a.md)       | [href](../tags/a_href.md)    |
| [\<area>](../tags/area.md) | [href](../tags/area_href.md) |
| [\<base>](../tags/base.md) | [href](../tags/base_href.md) |
| [\<link>](../tags/link.md) | [href](../tags/link_href.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### A 示例

href 属性指定 [\<a>](../tags/a.md) 链接的目的地：

```html idoc:preview:iframe
<a href="https://github.com/jaywcjlove/html-tutorial">访问 HTML Tutorial 仓库</a>
```

### Area 示例

带有可点击 [\<area>](../tags/area.md) 的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="../tags/a.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="../tags/abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="../tags/address.html">
</map>
```

### Base 示例

为页面上的所有相对 URL 指定一个 [\<base>](../tags/base.md) 基本 URL：

```html
<head>
  <base href="https://www.w3schools.com/images/">
</head>
```

### Link 示例

链接 [\<link>](../tags/link.md) 到外部样式表：

```html
<link rel="stylesheet" type="text/css" href="theme.css">
```

## 浏览器支持

`href` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<a>](../tags/a.md)       | Yes | Yes | Yes | Yes | Yes |
| [\<area>](../tags/area.md) | Yes | Yes | Yes | Yes | Yes |
| [\<base>](../tags/base.md) | Yes | Yes | Yes | Yes | Yes |
| [\<link>](../tags/link.md) | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg