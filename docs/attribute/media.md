HTML media 属性
===

## 定义和用法

`media` 属性指定链接文档针对什么媒体/设备进行优化。

此属性用于指定目标 URL 是为特殊设备（如 iPhone）、语音或印刷媒体设计的。

该属性可以接受多个值。

## 适用于

`media` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<a>](../tags/a.md)           | [media](../tags/a_media.md)      |
| [\<area>](../tags/area.md)     | [media](../tags/area_media.md)   |
| [\<link>](../tags/link.md)     | [media](../tags/link_media.md)   |
| [\<source>](../tags/source.md) | [media](../tags/source_media.md) |
| [\<style>](../tags/style.md)   | [media](../tags/style_media.md)  |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### A 示例

带有媒体属性的链接：

```html idoc:preview
<a href="../tags/a_media.html?output=print"
media="print and (resolution:300dpi)">
打开媒体属性页面进行打印。</a>
```

### Area 示例

带有可点击区域的图像地图：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126"
    media="screen and (min-color-index:256)" href="../tags/a.html" alt="Sun">
  <area shape="circle" coords="90,58,3"
    media="screen and (min-color-index:256)" href="../tags/address.html" alt="Mercury">
  <area shape="circle" coords="124,58,8"
    media="screen and (min-color-index:256)" href="../tags/applet.html" alt="Venus">
</map>
```

### Link 示例

两种不同媒体类型（屏幕和印刷）的两种不同样式表：

```html
<head>
  <link rel="stylesheet" type="text/css" href="theme.css">
  <link rel="stylesheet" type="text/css" href="print.css" media="print">
</head>
```

### Source 示例

媒体属性的使用：

```html
<source src="movie.ogg" type="video/ogg" media="screen and (min-width:320px)">
```

### Style 示例

指定用于打印的样式：

```html
<style media="print">
  h1 { color:#000000; }
  p { color:#000000; }
  body { background-color:#FFFFFF; }
</style>
```

## 浏览器支持

`media` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<a>](../tags/a.md)            | Yes           | Yes           | Yes           | Yes           | Yes           |
| [\<area>](../tags/area.md)      | Yes           | Yes           | Yes           | Yes           | Yes           |
| [\<link>](../tags/link.md)      | Yes           | Yes           | Yes           | Yes           | Yes           |
| [\<source>](../tags/source.md)  | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
| [\<style>](../tags/style.md)    | Yes           | Yes           | Yes           | Yes           | Yes           |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg