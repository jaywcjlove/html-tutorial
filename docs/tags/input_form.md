HTML \<input> form 属性
===

## 示例

位于 HTML 表单之外的输入字段（但仍然是表单的一部分）：

```html
<form action="/action_page.php" id="form1">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
</form>

<label for="lname">姓:</label>
<input type="text" id="lname" name="lname" form="form1">
```

```html idoc:preview:iframe
<form action="/action_page.php" id="form1">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit"><br><br>
</form>
下面的“姓氏”字段在表单元素之外，但仍然是表单的一部分。<br>
<label for="lname">姓:</label>
<input type="text" id="lname" name="lname" form="form1">
```

## 定义和用法

`form` 属性指定 `<input>` 元素所属的表单。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| form      | Yes | Yes | Yes | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input form="form_id">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *form\_id* | 指定 \<input> 元素所属的表单元素。 此属性的值必须是同一文档中 \<form> 元素的 id 属性。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
