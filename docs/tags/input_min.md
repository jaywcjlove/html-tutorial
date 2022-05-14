HTML \<input> min 属性
===

## 示例

使用 min 和 [max](./input_max.md) 属性：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="datemax">输入 1980-01-01 之前的日期：</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>
  <label for="datemin">输入 2000-01-01 之后的日期：</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  <label for="quantity">数量（1 到 5 之间）：</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>
  <input type="submit" value="提交">
</form>
```


## 定义和用法

`min` 属性指定 `<input>` 元素的最小值。

**提示：** 使用 `min` 属性和 `max` 属性来创建一系列合法值。

**注意：** `max` 和 `min` 属性适用于以下输入类型：数字、范围、日期、本地日期时间、月、时间和周。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| min       | 5.0 | 10.0 | 16.0 | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input min="number|date">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | 指定允许的最小值 |
| *date*   | 指定允许的最短日期 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg



