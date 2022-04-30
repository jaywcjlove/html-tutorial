HTML \<input type="month">
===

## 示例

将图像定义为提交按钮：

```html idoc:preview:iframe
<label for="bdaymonth">Birthday (month and year):</label>
<input type="month" id="bdaymonth" name="bdaymonth">
```

## 定义和用法

`<input type="month">` 定义了月份和年份控件。

格式为“YYYY-MM”。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="month" | 25.0 | 12.0 | Not supported | Not supported | 10.1 |

## 语法

```html
<input type="month">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg