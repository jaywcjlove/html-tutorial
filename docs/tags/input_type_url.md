HTML \<input type="url">
===

## 示例

定义一个用于输入 URL 的字段：

```html idoc:preview:iframe
<label for="homepage">Add your homepage:</label>
<input type="url" id="homepage" name="homepage">
```

## 定义和用法

`<input type="url">` 定义了一个用于输入 URL 的字段。

在提交表单之前会自动验证输入值。

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="url" | Yes | 10.0 | Yes | Yes | 10.1 |

## 语法

```html
<input type="url">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg