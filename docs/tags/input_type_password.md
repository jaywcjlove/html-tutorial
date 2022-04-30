HTML \<input type="password">
===

## 示例

定义一个用于输入数字的字段（您还可以设置接受哪些数字的限制）：

```html idoc:preview:iframe
<label for="pwd">Password:</label>
<input type="password" id="pwd" name="pwd">
```

## 定义和用法

`<input type="password">` 定义了一个密码字段（字符被屏蔽）。

**注意：** 任何涉及敏感信息（如密码）的表格都应通过 HTTPS 提供。

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="password" | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<input type="password">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg