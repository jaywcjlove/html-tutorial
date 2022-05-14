HTML \<input> readonly 属性
===

## 示例

带有只读输入字段的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="country">国家:</label>
  <input type="text" id="country" name="country" value="Norway" readonly><br><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`readonly` 属性是一个布尔属性。

如果存在，它指定输入字段是只读的。

不能修改只读输入字段（但是，用户可以通过 Tab 键选择它、突出显示它并从中复制文本）。

可以设置 `readonly` 属性以防止用户更改值，直到满足其他一些条件（例如选择复选框等）。 然后，JavaScript 可以删除只读值，并使输入字段可编辑。

**注意：** 表单仍会提交只读的输入字段，但不会提交已禁用的输入字段！

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| readonly  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input readonly>
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg