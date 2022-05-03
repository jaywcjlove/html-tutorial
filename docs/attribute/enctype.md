HTML enctype 属性
===

## 定义和用法

`enctype` 属性指定表单数据在提交到服务器时应如何编码。

**注意：** 只有在 `method="post"` 时才能使用 `enctype` 属性。

## 适用于

`enctype` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md) | [enctype](../tags/form_enctype.md) |

## 示例

发送编码为“multipart/form-data”的表单数据：

```html idoc:preview:iframe
<form action="/action_page_binary.asp" method="post" enctype="multipart/form-data">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| enctype   | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
