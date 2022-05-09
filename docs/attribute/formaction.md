HTML formaction 属性
===

## 定义和用法

`formaction` 属性指定提交表单时将表单数据发送到何处。 此属性覆盖表单的 `action` 属性。

`formaction` 属性仅用于具有 `type="submit"` 的输入/按钮。

## 适用于

`formaction` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<button>](../tags/button.md) | [formaction](../tags/button_formaction.md) |
| [\<input>](../tags/input.md)   | [formaction](../tags/input_formaction.md)  |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Button 示例

带有两个提交按钮的表单。 第一个提交按钮将表单数据提交到“action\_page.php”，第二个提交到“action\_page2.php”：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <button type="submit">Submit</button><br>
  <button type="submit" formaction="/action_page2.php">Submit to another page</button>
</form>
```

### Input 示例

具有两个提交按钮的 HTML 表单，具有不同的操作：

```html idoc:preview:iframe
<form action="/action_page.php">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit"><br>
  <input type="submit" formaction="/action_page2.php" value="Submit to another page">
</form>
```

## 浏览器支持

`formaction` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<button>](../tags/button.md) | 9.0 | 10.0 | 4.0 | 5.1 | 10.6 |
| [\<input>](../tags/input.md)   | 9.0 | 10.0 | 4.0 | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
