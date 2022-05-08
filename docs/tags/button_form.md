HTML \<button> form 属性
===

## 示例

位于表单外部的按钮（但仍然是表单的一部分）：

```HTML idoc:preview:iframe
<form action="/action_page.php" method="get" id="form1">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname">
</form>
<button type="submit" form="form1" value="Submit">Submit</button>
```

## 定义和用法

`form` 属性指定按钮所属的表单。

此属性的值必须等于同一文档中 `<form>` 元素的 `id` 属性。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| form      | 10.0 | 16.0 | 4.0 | 5.1 | 9.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button form="form_id">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *form\_id* | 指定 \<button> 元素所属的表单元素。 此属性的值必须是同一文档中 \<form> 元素的 id 属性。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg