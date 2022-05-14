HTML \<input> placeholder 属性
===

## 示例

带有占位符文本的电话输入字段：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="phone">输入电话号码:</label><br>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678"
  pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br>
  <small>Format: 123-45-678</small><br>
  <input type="submit">
</form> 
```


## 定义和用法

`placeholder` 属性指定描述输入字段的预期值的简短提示（例如，示例值或预期格式的简短描述）。

在用户输入值之前，简短提示会显示在输入字段中。

**注意：** `placeholder` 属性适用于以下输入类型：`text`, `search`, `url`, `tel`, `email`, 和 `password`。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| placeholder | 10.0 | 10.0 | 4.0 | 5.0 | 11.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input placeholder="text">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 指定描述输入字段预期值的简短提示 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

