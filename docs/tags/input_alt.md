HTML \<input> alt 属性
===

## 示例

带有代表提交按钮的图像的 HTML 表单：

```html
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname">
  <input type="image" src="../assets/chrome.svg" alt="Submit" width="48" height="48">
</form>
```

```html idoc:preview:iframe
单击图像，输入将被发送到服务器上名为 `/action_page.php` 的页面。
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname">
  <input type="image" src="../assets/chrome.svg" alt="Submit" width="48" height="48">
</form>
注意：图像输入类型默认发送激活图像按钮的单击的 X 和 Y 坐标。
```

## 定义和用法

`alt` 属性为用户提供替代文本，如果他/她由于某种原因无法查看图像（由于连接速度慢、src 属性中的错误，或者如果用户使用屏幕阅读器）。

**注意：** `alt` 属性只能与 [`<input type="image">`](./input_type_image.md) 一起使用。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| alt       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input alt="*text*">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 指定图像的替代文本 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
