HTML \<button> formtarget 属性
===

## 示例

带有两个提交按钮的表单。 第一个提交按钮使用默认目标（“\_self”）提交表单数据，第二个提交表单数据到新窗口（目标=“\_blank”）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <button type="submit" >提交</button>
  <button type="submit" formtarget="_blank">提交到新窗口</button>
</form>
```

## 定义和用法

`formtarget` 属性指定提交表单后在哪里显示响应。 此属性覆盖表单的 `target` 属性。

`formtarget` 属性仅用于具有 `type="submit"` 的按钮。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| formtarget | 9.0 | 10.0 | 4.0 | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="submit" formtarget="_blank|_self|_parent|_top|framename">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| _blank      | 在新窗口/选项卡中加载响应 |
| \_self      | 在同一帧中加载响应（这是默认设置） |
| \_parent    | 在父框架中加载响应 |
| \_top       | 在整个窗口中加载响应 |
| *framename* | 在命名的 iframe 中加载响应 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg