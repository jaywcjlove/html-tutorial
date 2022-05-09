HTML hreflang 属性
===

## 定义和用法

`hreflang` 属性指定链接文档的语言。

**注意：** 此属性仅供参考。

## 适用于

`hreflang` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<a>](../tags/a.md)       | [hreflang](../tags/a_hreflang.md)    |
| [\<area>](../tags/area.md) | [hreflang](../tags/area_hreflang.md) |
| [\<link>](../tags/link.md) | [hreflang](../tags/link_hreflang.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### A 示例

`hreflang` 属性指定链接中文档的语言：

```html idoc:preview:iframe
<a target="_blank" hreflang="en" href="https://github.com/jaywcjlove">HTML Tutorial</a>
```

### Area 示例

带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area hreflang="en" shape="rect" coords="34,44,270,350" alt="Computer" href="../tags/a.html">
  <area hreflang="en" shape="rect" coords="290,172,333,250" alt="Phone" href="../tags/abbr.html">
  <area hreflang="en" shape="circle" coords="337,300,44" alt="Cup of coffee" href="../tags/address.html">
</map>
```

### Link 示例

这里，hreflang 属性表示链接的文档是英文的：

```html
<link href="../tags/link.html" rel="parent" rev="subsection" hreflang="en">
```

## 浏览器支持

`hreflang` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<a>](../tags/a.md)        | Yes | Yes | Yes | Yes | Yes |
| [\<area>](../tags/area.md)  | Yes | Yes | Yes | Yes | Yes |
| [\<link>](../tags/link.md)  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
