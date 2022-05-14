HTML \<input> name 属性
===

## 示例

具有三个输入字段的 HTML 表单； 两个文本字段和一个提交按钮：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="提交">
</form>
```


## 定义和用法

`name` 属性指定了 `<input>` 元素的名称。

`name` 属性用于引用 JavaScript 中的元素，或在提交表单后引用表单数据。

**注意：** 只有具有 `name` 属性的表单元素才会在提交表单时传递其值。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| name      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input name="text">
```

## Attribute Values

| Value  | Description                                |
| ------ | ------------------------------------------ |
| *text* | Specifies the name of the \<input> element |

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
