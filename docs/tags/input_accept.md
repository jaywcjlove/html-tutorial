HTML \<input> accept 属性
===

## 示例

指定用户可以从文件输入对话框中选择的文件类型：

```html
<form action="/action_page.php">
  <label for="img">选择图片：</label>
  <input type="file" id="img" name="img" accept="image/*">
  <input type="submit">
</form>
```

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="img">选择图片：</label>
  <input type="file" id="img" name="img" accept="image/*">
  <input type="submit">
</form>
服务器处理您的输入并答案。
```

## 定义和使用

`accept` 属性指定用户可以从文件输入对话框中选择的文件类型的过滤器。

**注意：** `accept` 属性只能与 [`<input type="file">`](./input_type_file.md) 一起使用。

**提示：** 不要将此属性用作验证工具。 文件上传应在服务器上进行验证。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| accept    | 26.0 | 10.0 | 37.0 | 11.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input accept="file_extension|audio|video|image|media_type">
```

**提示：** 要指定多个值，请用逗号分隔这些值（例如 `<input accept="audio/*,video/*,image/*" />`。

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *file\_extension* | 指定用户可以选择的文件扩展名（例如：.gif、.jpg、.png、.doc） |
| audio/\*          | 用户可以选择所有声音文件 |
| video/\*          | 用户可以选择所有视频文件 |
| image/\*          | 用户可以选择所有图像文件 |
| *media\_type*     | 有效的媒体类型，没有参数。 查看 [IANA 媒体类型](http://www.iana.org/assignments/media-types/) 了解标准媒体类型的完整列表 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
