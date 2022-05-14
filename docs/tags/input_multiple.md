HTML \<input> multiple 属性
===

## 示例

接受多个值的文件上传字段：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="files">选择多个文件:</label>
  <input type="file" id="files" name="files" multiple><br><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`multiple` 属性是一个布尔属性。

如果存在，它指定允许用户在 `<input>` 元素中输入多个值。

**注意：** `multiple` 属性适用于以下输入类型：电子邮件和文件。

**提示：** 对于 [`<input type="file">`](./input_type_file.md)：要选择多个文件，请在选择时按住 CTRL 或 SHIFT 键。

**提示：** 对于 [`<input type="email">`](./input_type_email.md)：用逗号分隔每封电子邮件，例如：电子邮件字段中的值 `mail@example.com`,`mail2@example.com`,`mail3@example.com`。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| multiple  | 6.0 | 10.0 | 3.6 | 5.0 | 11.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input multiple>
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
