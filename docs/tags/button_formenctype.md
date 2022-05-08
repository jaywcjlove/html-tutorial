HTML \<button> formenctype 属性
===

## 示例

带有两个提交按钮的表单。 第一个提交按钮使用默认字符编码提交表单数据，第二个提交不使用字符编码的表单数据：

```html idoc:preview:iframe
<form action="/action_page_binary.asp" method="post">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname" value="Ståle"><br><br>
  <button type="submit">Submit with character encoding</button>
  <button type="submit" formenctype="text/plain">Submit without character encoding</button>
</form>
```

## 定义和用法

`formenctype` 属性指定表单数据在发送到服务器之前应如何编码。 此属性覆盖表单的 `enctype` 属性。

`formenctype` 属性仅用于具有 `type="submit"` 的按钮。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| formenctype | 9.0 | 10.0 | 4.0 | 5.1 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="submit" formenctype="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| application/x-www-form-urlencoded | 默认。 所有字符在发送前都会被编码 |
| multipart/form-data               | 如果用户将通过表单上传文件，则此值是必需的 |
| text/plain                        | 发送完全没有任何编码的数据。 不建议 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg