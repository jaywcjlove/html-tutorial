HTML \<input> checked 属性
===

## 示例

带有预选复选框的 HTML 表单：

```html
<form action="/action_page.php">
  <input type="checkbox" name="vehicle1" value="Bike">
  <label for="vehicle1"> 我有一辆自行车</label><br>
  <input type="checkbox" name="vehicle2" value="Car">
  <label for="vehicle2"> 我有一辆车</label><br>
  <input type="checkbox" name="vehicle3" value="Boat" checked>
  <label for="vehicle3"> 我有一条船</label><br><br>
  <input type="submit" value="Submit">
</form>
```

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <input type="checkbox" name="vehicle1" value="Bike">
  <label for="vehicle1"> 我有一辆自行车</label><br>
  <input type="checkbox" name="vehicle2" value="Car">
  <label for="vehicle2"> 我有一辆车</label><br>
  <input type="checkbox" name="vehicle3" value="Boat" checked>
  <label for="vehicle3"> 我有一条船</label><br><br>
  <input type="submit" value="Submit">
</form>
```

## 定义和用法

`checked` 属性是一个布尔属性。

如果存在，它指定在页面加载时应该预先选择（检查）一个 `<input>` 元素。

`checked` 属性可以与 `<input type="checkbox">` 和 `<input type="radio">` 一起使用。

`checked` 属性也可以在页面加载后使用 JavaScript 设置。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| checked   | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input checked>
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
