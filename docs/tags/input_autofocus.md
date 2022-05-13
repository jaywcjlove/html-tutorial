HTML \<input> autofocus 属性
===

## 示例

让“名字”输入字段在页面加载时自动获得焦点：

```html
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname" autofocus><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit">
</form>
```

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname" autofocus><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit">
</form>
```

## 定义和用法

`autofocus` 属性是一个布尔属性。

如果存在，它指定 `<input>` 元素应在页面加载时自动获得焦点。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| autofocus | 5.0 | 11.0 | 4.0 | 5.0 | 9.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input autofocus>
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
