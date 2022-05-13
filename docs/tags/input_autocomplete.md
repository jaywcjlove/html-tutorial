HTML \<input> autocomplete 属性
===

## 示例

具有自动完成功能的 HTML 表单（一个输入字段关闭）：

```html idoc:preview:iframe
<form action="/action_page.php" autocomplete="on">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <label for="email">邮箱:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br>
  <input type="submit">
</form>
```

## 定义和用法

`autocomplete` 属性指定输入字段是否应启用自动完成功能。

自动完成允许浏览器预测值。 当用户开始输入字段时，浏览器应根据之前输入的值显示填充字段的选项。

**注意：** `autocomplete` 属性适用于以下输入类型： text, search, url, tel, email, password, datepickers, range, 和 color。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| autocomplete | 17.0 | 6.0 | 2.0 | 5.1 | 10.0 |


## 语法

```html
<input autocomplete="on|off">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| on    | 默认。 指定自动完成已打开（启用） |
| off   | 指定自动完成关闭（禁用） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
