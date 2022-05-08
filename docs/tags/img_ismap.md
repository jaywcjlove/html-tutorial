HTML \<img> ismap 属性
===

## 示例

服务器端图像映射，点击图标，点击坐标将作为 `URL` 查询字符串发送到 `/action_page.php` 服务器：

```html idoc:preview
<a href="/action_page.php">
  <img src="../assets/chrome.svg" alt="Chrome 浏览器" width="42" height="42" ismap>
</a>
```

## 定义和用法

`ismap` 属性是一个布尔属性。

当存在时，它指定图像是服务器端图像映射的一部分（图像映射是具有可点击区域的图像）。

单击服务器端图像地图时，单击坐标将作为 URL 查询字符串发送到服务器。

**注意：** 只有当 `<img>` 元素是具有有效 `href` 属性的 `<a>` 元素的后代时，才允许使用 `ismap` 属性。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| ismap     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img ismap>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
