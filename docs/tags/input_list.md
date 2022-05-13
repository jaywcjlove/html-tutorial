HTML \<input> list 属性
===

## 示例

在 \<datalist> 中具有预定义值的 \<input> 元素：

```html
<input list="browsers">
<datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Google Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="browser">从列表中选择您的浏览器：</label>
  <input list="browsers" name="browser" id="browser">
  <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
  <input type="submit" value="提交">
</form><br>
注意： Safari 12.0（或更早版本）不支持 datalist 标签。
```

## 定义和用法

`list` 属性指的是 `<datalist>` 元素，其中包含 `<input>` 元素的预定义选项。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| list      | 20.0 | 10.0 | 4.0 | Not supported | 9.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input list="datalist_id">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *datalist\_id* | 指定要将 \<input> 元素绑定到的数据列表的 id |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

