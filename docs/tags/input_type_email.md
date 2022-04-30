HTML \<input type="email">
===

## 示例

为电子邮件地址定义一个字段（提交时自动验证）：

```html idoc:preview:iframe
<label for="email">Enter your email:</label>
<input type="email" id="email" name="email">
```

## 定义和用法

`<input type="email">` 为电子邮件地址定义了一个字段。

输入值会自动验证，以确保它是格式正确的电子邮件地址。

要定义允许多个电子邮件地址的电子邮件字段，请添加“多个”属性。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="email" | 5.0 | 10.0 | 4.0 | 5.0 | 10.1 |

## 语法

```html
<input type="email">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg