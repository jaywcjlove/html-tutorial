HTML \<fieldset> form 属性
===

## 示例

位于表单外部的 \<fieldset> 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" id="form1">
  <label for="favcolor">什么是你最喜欢的颜色？</label>
  <input type="text" id="favcolor" name="favcolor">
  <input type="submit">
</form>

<fieldset form="form1">
  <legend>个人资料:</legend>
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname" form="form1"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname" form="form1">
</fieldset>
```

## 定义和用法

`form` 属性指定字段集所属的表单。

此属性的值必须等于同一文档中 `<form>` 元素的 `id` 属性。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| form      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<fieldset form="form_id">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *form\_id* | 指定 \<fieldset> 元素所属的表单元素。 此属性的值必须是同一文档中 \<form> 元素的 id 属性。 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
