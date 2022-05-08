HTML \<button> formaction 属性
===

## 示例

带有两个提交按钮的表单。 第一个提交按钮将表单数据提交到 `action_page.php`，第二个提交到 `action_page2.php`：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <button type="submit">Submit</button>
  <button type="submit" formaction="/action_page2.php">Submit to another page</button>
</form>
```

## 定义和用法

`formaction` 属性指定提交表单时将表单数据发送到何处。 此属性覆盖表单的 `action` 属性。

`formaction` 属性仅用于具有 `type="submit"` 的按钮。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| formaction | 9.0 | 10.0 | 4.0 | 5.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="submit" formaction="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定发送表单数据的位置。可能的值：<br>* 绝对 URL - 页面的完整地址（如 `href="http://www.example.com/formresult.asp"`） <br>* 相对 URL - 指向当前站点内的文件（如 `href="formresult.asp"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg