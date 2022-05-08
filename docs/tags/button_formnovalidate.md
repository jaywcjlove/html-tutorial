HTML \<button> formnovalidate 属性
===

## 示例

带有两个提交按钮的表单。 第一个提交按钮提交表单数据默认验证，第二个提交表单数据不验证：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email"><br><br>
  <button type="submit">提交</button>
  <button type="submit" formnovalidate>未经验证提交</button>
</form>
```

## 定义和用法

`formnovalidate` 属性是一个布尔属性。

如果存在，它指定不应在提交时验证表单数据。 此属性覆盖表单的 `novalidate` 属性。

`formnovalidate` 属性仅用于具有 `type="submit"` 的按钮。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| formnovalidate | 6.0 | 11.0 | 4.0 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="submit" formnovalidate>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg