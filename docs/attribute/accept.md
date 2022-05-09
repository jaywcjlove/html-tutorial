HTML accept 属性
===

## 定义和用法

accept 属性指定服务器接受的文件类型（可以通过文件上传提交）。

**注意：** accept 属性只能与 \<input type="file"> 一起使用。

**提示：** 不要将此属性用作验证工具。 文件上传应在服务器上进行验证。

## 适用于

`accept` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md) | [accept](../tags/input_accept.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## Input 示例

指定服务器只接受文件上传中的图片文件：

```html idoc:preview:iframe
<form action="/action_page.php">
  <input type="file" name="pic" accept="image/*">
  <input type="submit">
</form>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| accept    | 8.0 | 10.0 | 4.0 | 6.0 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg