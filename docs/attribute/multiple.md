HTML multiple 属性
===

## 定义和用法

`multiple` 属性是一个布尔属性。

当存在时，它指定允许用户输入/选择多个值。

## 适用于

`multiple` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md)   | [multiple](../tags/input_multiple.md)  |
| [\<select>](../tags/select.md) | [multiple](../tags/select_multiple.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Input 示例

接受多个值的文件上传字段：

```html idoc:preview:iframe
<form action="/action_page.php">
  Select images: <input type="file" name="img" multiple><br>
  <input type="submit">
</form>
```

### Select 示例

允许多项选择的下拉列表：

```html idoc:preview:iframe
<select multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

## 浏览器支持

`multiple` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<input>](../tags/input.md)   | 6.0 | 10.0 | 3.6 | 5.0 | 11.0 |
| [\<select>](../tags/select.md) | Yes | Yes  | Yes | Yes | Yes  |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg