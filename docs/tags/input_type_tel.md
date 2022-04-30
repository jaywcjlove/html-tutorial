HTML \<input type="tel">
===

## 示例

定义一个用于输入电话号码的字段：

```html idoc:preview:iframe
<label for="phone">Enter your phone number:</label>
<input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
```

## 定义和用法

`<input type="tel">` 定义了一个用于输入电话号码的字段。

**注意：** 不支持“tel”的浏览器会退回到标准的“文本”输入。

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="tel" | Yes | 10.0 | Yes | Yes | 11.0 |

## 语法

```html
<input type="tel">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg