HTML \<input> disabled 属性
===

## 示例

带有禁用输入字段的 HTML 表单：

```html
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname" disabled><br><br>
  <input type="submit" value="Submit">
</form>
```

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname" disabled><br><br>
  <input type="submit" value="Submit">
</form>
```


## 定义和用法

`disabled` 属性是一个布尔属性。

如果存在，它指定应该禁用 `<input>` 元素。

禁用的输入元素不可用且不可点击。

可以设置 `disabled` 属性以阻止用户使用 `<input>` 元素，直到满足某些其他条件（例如选择复选框等）。 然后，JavaScript 可以删除禁用的值，并使 `<input>` 元素可用。

**提示：** 表单中禁用的 `<input>` 元素将不会被提交！

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| disabled  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input disabled>
```


[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
