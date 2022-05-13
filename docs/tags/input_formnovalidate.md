HTML \<input> formnovalidate 属性
===

## 示例

第二个提交按钮覆盖表单的 HTTP 方法：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="email">输入您的邮箱:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="提交">
  <input type="submit" formnovalidate="formnovalidate" value="未经验证提交">
</form>
```

## 定义和用法

`formnovalidate` 属性是一个布尔属性。

如果存在，它指定 `<input>` 元素在提交时不应该被验证。

`formnovalidate` 属性覆盖了 `<form>` 元素的 `novalidate` 属性。

**注意：** `formnovalidate` 属性可以与 [`type="submit"`](./input_type_submit.md) 一起使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| formnovalidate | Yes | 10.0 | Yes | 10.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input formnovalidate="formnovalidate">
```

**注意：** formnovalidate 属性为布尔属性，可以通过以下方式设置：

```html
<input formnovalidate>
<input formnovalidate="formnovalidate">
<input formnovalidate="">
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

