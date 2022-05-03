HTML novalidate 属性
===

## 定义和用法

`novalidate` 属性是一个布尔属性。

当存在时，它指定表单数据（输入）在提交时不应该被验证。

## 适用于

`novalidate` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md) | [novalidate](../tags/form_novalidate.md) |

## 示例

指示表单在提交时不被验证：

```html idoc:preview:iframe
<form action="/action_page.php" novalidate>
  E-mail: <input type="email" name="user_email">
  <input type="submit">
</form>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| novalidate | 10.0 | 10.0 | 4.0 | ❌ 不支持 | 10.6 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg