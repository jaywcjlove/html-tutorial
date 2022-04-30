HTML \<input type="datetime-local">
===

## 示例

显示日期和时间控件（无时区）：

```html idoc:preview:iframe
<label for="birthdaytime">Birthday (date and time):</label>
<input type="datetime-local" id="birthdaytime" name="birthdaytime">
```

## 定义和用法

`<input type="datetime-local">` 定义了一个日期选择器。

结果值包括年、月、日和时间。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="datetime-local" | 20.0 | 12.0 | 93.0 | 14.1 | 11.0 |

## 语法

```html
<input type="datetime-local">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg