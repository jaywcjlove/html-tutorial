HTML \<button> type 属性
===

## 示例

两个按钮元素充当一个提交按钮和一个重置按钮（在表单中）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <button type="submit" value="Submit">提交</button>
  <button type="reset" value="Reset">重置</button>
</form>
```

## 定义和用法

`type` 属性指定按钮的类型。

**提示：** 始终为 `<button>` 元素指定 type 属性。 不同的浏览器可能对 `<button>` 元素使用不同的默认类型。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| type      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="button|submit|reset">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| button | 该按钮是一个可点击的按钮 |
| submit | 该按钮是一个提交按钮（提交表单数据） |
| reset  | 该按钮是一个重置按钮（将表单数据重置为其初始值） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg