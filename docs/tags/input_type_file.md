HTML \<input type="file">
===

## 示例

为电子邮件地址定义一个字段（提交时自动验证）：

```html idoc:preview:iframe
<label for="myfile">Select a file:</label>
<input type="file" id="myfile" name="myfile">
```

## 定义和用法

`<input type="file">` 定义了一个文件选择字段和一个用于文件上传的“浏览”按钮。

要定义允许选择多个文件的文件选择字段，请添加 `multiple` 属性。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="file" | 1.0 | Yes | 1.0 | 1.0 | 1.0 |

## 语法

```html
<input type="file">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg