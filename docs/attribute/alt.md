HTML alt 属性
===

## 定义和用法

如果用户由于某种原因无法查看图像（由于连接速度慢、src 属性中的错误或用户使用屏幕阅读器），则 alt 属性提供图像的替代信息。

**注意：** [\<img>](../tags/img.md) 元素需要 alt 属性。

**注意：** 对于 [\<input>](../tags/input.md) 元素，alt 属性只能与 [\<input type="image">](../tags/input_type_image.md) 一起使用。

**提示：** 要为图像创建工具提示，请使用 [title](../reference/standardattributes.md) 属性！

## 适用于

`alt` 属性可用于以下元素：

| 标签 Element | 属性 Attribute |
| ----- | ----- |
| [\<area>](../tags/area.md)   | [alt](../tags/area_alt.md)  |
| [\<img>](../tags/img.md)     | [alt](../tags/img_alt.md)   |
| [\<input>](../tags/input.md) | [alt](../tags/input_alt.md) |

## 示例

### Area 示例

带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="a.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```

### Img 示例

图片找不到，指定 `alt` 内容替代文本的图像：

```html idoc:preview:iframe
<img src="smiley.gif" alt="Smiley face">
```

### Input 示例

带有代表提交按钮的图像的 HTML 表单，图片不存在显示 `alt` 内容：

```html idoc:preview:iframe
<form action="/action_page.php">
  First name: <input type="text" name="fname"><br>
  <input type="image" src="submit.gif" alt="Submit" width="48" height="48">
</form>
```

## 浏览器支持

`alt` 属性对每个元素都有以下浏览器支持：

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| area    | Yes | Yes | Yes | Yes | Yes |
| img     | Yes | Yes | Yes | Yes | Yes |
| input   | Yes | Yes | Yes | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg