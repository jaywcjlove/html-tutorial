HTML \<form> novalidate 属性
===

## 示例

指示表单在提交时不被验证：

```html idoc:preview:iframe
<form action="/action_page.php" novalidate>
  <label for="email">输入您的邮箱:</label>
  <input type="email" id="email" name="email"><br>
  <input type="submit">
</form>
```

## 定义和用法

`novalidate` 属性是一个布尔属性。

当存在时，它指定表单数据（input）在提交时不应该被验证。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| novalidate | Yes | 10.0 | 4.0 | 10.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form novalidate>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
