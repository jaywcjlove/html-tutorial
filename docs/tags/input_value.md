HTML \<input> value 属性
===

## 示例

具有初始（默认）值的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname" value="三"><br>
  <label for="lname">姓氏:</label>
  <input type="text" id="lname" name="lname" value="张"><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`value` 属性指定 `<input>` 元素的值。

`value` 属性用于不同的输入类型：

* 对于 `button`、`reset` 和 `submit`——它定义了按钮上的文本
* 对于 `text`、`password` 和 `hidden` - 它定义了输入字段的初始（默认）值
* 对于 `checkbox`、`radio`、`image` - 它定义了与输入关联的值（这也是提交时发送的值）

**Note:** `value` 属性不能与 `<input type="file">` 一起使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| value     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input value="text">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 指定 \<input> 元素的值 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

