HTML \<form> action 属性
===

## 示例

提交时，将表单数据发送到名为“action\_page.php”的文件（以处理输入）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`action` 属性指定提交表单时将表单数据发送到何处。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| action    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form action="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 提交表单时将表单数据发送到何处。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `action="http://www.example.com/example.htm"`） <br>* 相对 URL - 指向网站内的文件（如 `action="example.htm"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
