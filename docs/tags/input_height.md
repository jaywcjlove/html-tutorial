HTML \<input> height 属性
===

## 示例

定义一个图像作为提交按钮，具有高度和宽度属性：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="image" src="../assets/chrome.svg" alt="Submit" width="48" height="48"  formtarget="_blank"><br>
  点击👆上面图标提交
</form>
```

## 定义和用法

`height` 属性指定了 `<input>` 元素的高度。

**注意：** `height` 属性仅与 `<input type="image">` 一起使用。

**提示：** 始终为图像指定 `height` 和 `width` 属性。 如果设置了高度和宽度，则在加载页面时保留图像所需的空间。 但是，如果没有这些属性，浏览器将不知道图像的大小，也无法为其预留适当的空间。 效果将是页面布局将在加载期间更改（同时加载图像）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| height    | Yes | Yes | 16.0 | Yes | Yes |

## 语法

```html
<input height="pixels">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *pixels* | 以像素为单位的高度（例如 height="100"） |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

