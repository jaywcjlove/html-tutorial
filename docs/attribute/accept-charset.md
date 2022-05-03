HTML accept-charset 属性
===

## 定义和用法

`accept-charset` 属性指定要用于表单提交的字符编码。

默认值为保留字符串“UNKNOWN”（表示编码等于包含 [\<form>](../tags/form.md) 元素的文档的编码）。

## 适用于

`accept-charset` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md) | [accept-charset](../tags/form_accept_charset.md) |

### Form 示例

具有 accept-charset 属性的表单：

```html idoc:preview:iframe
<form action="/action_page.php" accept-charset="ISO-8859-1">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| accept-charset | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg