HTML download 属性
===

## 定义和用法

`download` 属性指定当用户单击超链接时将下载目标。

仅当设置了 href 属性时才使用此属性。

`download` 属性的值将是下载文件的新名称。 对允许值没有限制，浏览器会自动检测正确的文件扩展名并将其添加到文件中（`.img`、`.pdf`、`.txt`、`.html` 等）。

如果省略该值，则使用原始文件名。

## 适用于

The `download` attribute can be used on the following elements:

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<a>](../tags/a.md)       | [download](../tags/a_download.md)    |
| [\<area>](../tags/area.md) | [download](../tags/area_download.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

单击链接时下载文件（而不是导航到文件）：

```html idoc:preview:iframe
<a href="../assets/workplace.jpg" download>下载 workplace.jpg</a>
```

### Area 示例

单击时将下载的带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="../tags/a.html" download="Computer">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="../tags/abbr.html" download="Phone">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="../tags/address.html" download="Cup of coffee">
</map>
```

## 浏览器支持

`download` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<a>](../tags/a.md)       | 14.0 | 13.0          | 20.0 | ❌ 不支持 | 15.0 |
| [\<area>](../tags/area.md) | 14.0 | ❌ 不支持 | 20.0 | ❌ 不支持 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
