HTML \<fieldset> disabled 属性
===

## 示例

禁用一组相关的表单元素：

```html idoc:preview:iframe
<form action="/action_page.php">
  <fieldset disabled>
    <legend>个人资料:</legend>
    <label for="fname">名:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">姓:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <label for="email">邮箱:</label>
    <input type="email" id="email" name="email"><br><br>
    <label for="birthday">生日:</label>
    <input type="date" id="birthday" name="birthday"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

## 定义和用法

`disabled` 属性是一个布尔属性。

当存在时，它指定一组相关的表单元素（字段集）应该被禁用。

禁用的字段集不可用且不可点击。

可以设置 `disabled` 属性以阻止用户使用字段，直到满足某些其他条件（例如选择复选框等）。 然后，JavaScript 可以删除禁用的值，并使字段集再次可用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| disabled  | Yes | Yes | Yes | 6.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<fieldset disabled>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
