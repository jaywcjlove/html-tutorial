HTML \<form> accept-charset 属性
===

## 示例

具有 `accept-charset` 属性的表单：

```html idoc:preview:iframe
<form action="/action_page.php" accept-charset="utf-8">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <input type="submit" value="提交">
</form>
```

## 定义和使用

`accept-charset` 属性指定要用于表单提交的字符编码。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| accept-charset | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form accept-charset="character_set">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *character\_set* | 用于表单提交的一个或多个字符编码的空格分隔列表。常用值：<br>* UTF-8 - Unicode 字符编码 <br>* ISO-8859-1 - 拉丁字母的字符编码理论上，任何字符编码都可以使用，但没有浏览器能理解所有这些。 字符编码使用得越广泛，浏览器理解它的机会就越大。要查看所有可用的字符编码，请转到我们的 [字符集参考](ref_charactersets.asp)。|
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
