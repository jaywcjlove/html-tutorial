HTML \<input> formtarget 属性
===

## 示例

具有两个提交按钮的表单，具有不同的目标窗口：

```html idoc:preview:iframe
<form action="/action_page.php">
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="正常提交">
  <input type="submit" formtarget="_blank" value="提交到新窗口">
</form>
```

## 定义和用法

`formtarget` 属性指定一个名称或关键字，指示在哪里显示提交表单后收到的响应。

`formtarget` 属性覆盖了 `<form>` 元素的 `target` 属性。

**注意：** `formtarget` 属性可以与 `type="submit"` 和 `type="image"` 一起使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| formtarget | Yes | 10.0 | Yes | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input formtarget="_blank|_self|_parent|_top|framename">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| \_blank     | 响应显示在新窗口或选项卡中 |
| \_self      | 响应显示在同一帧中（这是默认设置） |
| \_parent    | 响应显示在父框架中 |
| \_top       | 响应显示在整个窗口中 |
| *framename* | 响应显示在命名的 iframe 中 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
