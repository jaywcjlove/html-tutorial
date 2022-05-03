HTML list 属性
===

## 定义和用法

`list` 属性指的是 [`<datalist>`](../tags/datalist.md) 元素，其中包含 [`<input>`](../tags/input.md) 元素的预定义选项。

## 适用于

`list` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md) | [list](../tags/input_list.md) |

## 示例

在 [`<datalist>`](../tags/datalist.md) 中具有预定义值的 [\<input>](../tags/input.md) 元素：

```html idoc:preview:iframe
<input list="browsers">

<datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Google Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| list      | 20.0 | 10.0 | 4.0 | Not supported | 9.6 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg