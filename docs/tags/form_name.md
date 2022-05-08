HTML \<form> name 属性
===

## 示例

具有 name 属性的 HTML 表单：

```html idoc:preview:iframe
<script>
  function formSubmit() {
    document.forms["myForm"].submit();
  }
</script>
<form action="/action_page.php" method="get" name="myForm">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="button" onclick="formSubmit()" value="Send form data!">
</form>
```

## 定义和用法

`name` 属性指定表单的名称。

`name` 属性用于引用 JavaScript 中的元素，或在提交表单后引用表单数据。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| name      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


## 语法

```html
<form name="text">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 指定表单的名称 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

