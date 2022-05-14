HTML \<input> step 属性
===

## 示例

具有指定合法数字间隔的输入字段的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="points">积分:</label>
  <input type="number" id="points" name="points" step="3">
  <input type="submit">
</form>
```


## 定义和用法

`step` 属性指定 `<input>` 元素中合法数字之间的间隔。

示例：如果 `step="3"`，则合法数字可以是 -3、0、3、6 等。

**提示：** `step` 属性可以与 `max` 和 `min` 属性一起使用，以创建一系列合法值。

**注意：** `step` 属性适用于以下输入类型：数字、范围、日期、本地日期时间、月、时间和周。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| step      | 6.0 | 10.0 | 16.0 | 5.0 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input step="number">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | 指定输入字段中合法数字之间的间隔。 默认为 1 |
| any |   |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
