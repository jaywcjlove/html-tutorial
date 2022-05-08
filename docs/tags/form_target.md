HTML \<form> target 属性
===

## 示例

在新窗口或选项卡中显示收到的响应：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" target="_blank">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`target` 属性指定一个名称或关键字，指示在哪里显示提交表单后收到的响应。

`target` 属性定义了浏览上下文（例如选项卡、窗口或内联框架）的名称或关键字。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| target    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form target="_blank|_self|_parent|_top*|framename">
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

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
