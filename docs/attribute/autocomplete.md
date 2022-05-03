HTML autocomplete 属性
===

## 定义和用法

`autocomplete` 属性指定表单或输入字段是否应该打开或关闭自动完成功能。

自动完成允许浏览器预测值。 当用户开始输入字段时，浏览器应根据之前输入的值显示填充字段的选项。

**提示：** 可以为表单设置“开启”自动完成功能，为特定输入字段设置“关闭”功能，反之亦然。

**注意：** `autocomplete` 属性适用于以下 [`<input>`](../tags/input.md) 类型：[文本](../tags/input_type_text.md)、[搜索](../tags/input_type_search.md)、[url](../tags/input_type_url.md)、[电话](../tags/input_type_tel.md)、[电子邮件](../tags/input_type_email.md)、[密码](../tags/input_type_password.md)、[日期选择器](../tags/input_type_date.md)、[范围](../tags/input_type_range.md)和[颜色](../tags/input_type_color.md)。

## 适用于

`autocomplete` 属性可用于以下元素：

| 标签 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md)   | [autocomplete](../tags/form_autocomplete.md)  |
| [\<input>](../tags/input.md) | [autocomplete](../tags/input_autocomplete.md) |

## 示例

### Form 示例

具有自动完成功能的表单：

```html idoc:preview:iframe
<form action="/action\_page.php" method="get" autocomplete="on">
  First name:<input type="text" name="fname"><br>
  E-mail: <input type="email" name="email"><br>
  <input type="submit">
</form>
```

### Input 示例

具有自动完成功能的 HTML 表单（一个输入字段关闭）：

```html idoc:preview:iframe
<form action="/action_page.php" autocomplete="on">
  First name:<input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  E-mail: <input type="email" name="email" autocomplete="off"><br>
  <input type="submit">
</form>
```

## 浏览器支持

`autocomplete` 属性对每个元素都有以下浏览器支持：

| 标签 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [form](../tags/form.md)    | Yes  | Yes | 4.0 | 5.2 | 15.0 |
| [input](../tags/input.md)   | 17.0 | 5.0 | 4.0 | 5.2 | 9.6  |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg