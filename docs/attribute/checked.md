HTML checked 属性
===

## 定义和用法

`checked` 属性是一个布尔属性。

如果存在，它指定在页面加载时应该预先选择（检查）一个 [`<input>`](../tags/input.md) 元素。

`checked` 属性可以与 [`<input type="checkbox">`](../tags/input_type_checkbox.md) 和 [`<input type="radio">`](../tags/input_type_radio.md) 一起使用。

`checked` 属性也可以在页面加载后使用 JavaScript 设置。

## 适用于

`checked` 属性可用于以下元素：

| 标签 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md) | [checked](../tags/input_checked.md) |

## 示例

带有预选复选框的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <input type="checkbox" name="vehicle" value="Bike"> I have a bike<br>
  <input type="checkbox" name="vehicle" value="Car" checked> I have a car<br>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| checked   | 1.0 | 2.0 | 1.0 | 1.0 | 1.0 |



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg