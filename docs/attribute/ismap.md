HTML ismap 属性
===

## 定义和用法

`ismap` 属性是一个布尔属性。

当存在时，它指定图像是服务器端图像映射的一部分（图像映射是具有可点击区域的图像）。

单击服务器端图像地图时，单击坐标将作为 URL 查询字符串发送到服务器。

**注意：** 只有当 `<img>` 元素是具有有效 `href` 属性的 `<a>` 元素的后代时，才允许使用 `ismap` 属性。

## 适用于

`ismap` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<img>](../tags/img.md) | [ismap](../tags/img_ismap.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

服务器端图像映射：

```html idoc:preview:iframe
<a href="/action_page.php">
  <img src="../assets/editors-001.png" alt="穿夹克的女孩t" ismap height="300">
</a>
```
<!--rehype:style=min-height: 300px;-->

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| ismap     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg