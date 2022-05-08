HTML \<form> autocomplete 属性
===

## 示例

具有自动完成功能的表单：

```html idoc:preview:iframe
<form action="/action_page.php" autocomplete="on" method="get">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="email">Email:</label>
  <input type="text" id="email" name="email"><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`autocomplete` 属性指定表单是否应该打开或关闭自动完成功能。

启用自动完成后，浏览器会根据用户之前输入的值自动完成值。

**提示：** 可以为表单设置“开启”自动完成功能，为特定输入字段设置“关闭”功能，反之亦然。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| autocomplete | Yes | Yes | 4.0 | 5.2 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form autocomplete="on|off">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| on    | 默认。 浏览器将根据用户之前输入的值自动完成值 |
| off   | 用户每次使用都必须在每个字段中输入一个值。 浏览器不会自动完成条目 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

