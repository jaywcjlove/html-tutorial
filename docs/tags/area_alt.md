HTML \<area> alt 属性
===

## 示例

使用 alt 属性为图像映射中的每个区域指定替代文本：

```html idoc:preview
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="a.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```
<!--rehype:style=min-height: 280px;-->

## 定义和用法

如果图像无法显示，`alt` 属性指定区域的替代文本。

如果用户由于某种原因无法查看图像（由于连接速度慢、src 属性中的错误或用户使用屏幕阅读器），`alt` 属性会为图像提供替代信息。

如果存在 `href` 属性，则需要 `alt` 属性。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| alt       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area alt="text">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 如果图像无法显示，则指定该区域的替代文本 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg