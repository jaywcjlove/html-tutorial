HTML \<input> formenctype 属性
===

## 示例

发送默认编码的表单数据（第一个提交按钮），并编码为 `multipart/form-data`（第二个提交按钮）：

```html idoc:preview:iframe
<form action="/action_page_binary.asp" method="post">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="提交">
  <input type="submit" formenctype="multipart/form-data" value="提交为 Multipart/form-data">
</form>
```

## 定义和用法

`formenctype` 属性指定表单数据在提交到服务器时应如何编码（仅适用于具有 `method="post"` 的表单）

`formenctype` 属性覆盖了 `<form>` 元素的 `enctype` 属性。

**注意：** `formenctype` 属性与 `type="submit"` 和 `type="image"` 一起使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| formenctype | Yes | 10.0 | Yes | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input formenctype="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| application/x-www-form-urlencoded | 默认。 所有字符在发送前都经过编码（空格转换为“+”符号，特殊字符转换为 ASCII HEX 值） |
| multipart/form-data               | 如果用户将通过表单上传文件，则此值是必需的 |
| text/plain                        | 发送完全没有任何编码的数据。 不建议 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

