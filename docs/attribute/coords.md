HTML coords 属性
===

## 定义和用法

`coords` 属性指定图像地图中某个区域的坐标。

`coords` 属性与 [`shape`](./shape.md) 属性一起使用来指定区域的大小、形状和位置。

**提示：** 区域左上角的坐标为 `0,0`。

## 适用于

`coords` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<area>](../tags/area.md) | [coords](../tags/area_coords.md) |

## 示例

带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="../tags/a.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="../tags/abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="../tags/address.html">
</map>
```
<!--rehype:style=height: 330px;-->

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| coords    | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg