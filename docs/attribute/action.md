HTML action 属性
===

## 定义和用法

`action` 属性指定提交表单时将表单数据发送到何处。

## 适用于

`action` 属性可用于以下元素：

| 标签 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md) | [action](../tags/form_action.md) |

## 示例

提交时，将表单数据发送到名为 `/action_page.php` 的文件（以处理输入）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| action    | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
