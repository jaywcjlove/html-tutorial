HTML form 属性
===

## 定义和用法

`form` 属性指定元素所属的形式。

此属性的值必须等于同一文档中 `<form>` 元素的 `id` 属性。

## 适用于

`form` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<button>](../tags/button.md)     | [form](../tags/button_form.md)   |
| [\<fieldset>](../tags/fieldset.md) | [form](../tags/fieldset_form.md) |
| [\<input>](../tags/input.md)       | [form](../tags/input_form.md)    |
| [\<label>](../tags/label.md)       | [form](../tags/label_form.md)    |
| [\<meter>](../tags/meter.md)       | [form](../tags/meter_form.md)    |
| [\<object>](../tags/object.md)     | [form](../tags/object_form.md)   |
| [\<output>](../tags/output.md)     | [form](../tags/output_form.md)   |
| [\<select>](../tags/select.md)     | [form](../tags/select_form.md)   |
| [\<textarea>](../tags/textarea.md) | [form](../tags/textarea_form.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Button 示例

位于表单外部的按钮（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" id="form1">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
</form>

<button type="submit" form="form1" value="Submit">Submit</button>
```

### Fieldset 示例

位于表单外部的 [\<fieldset>](../tags/fieldset.md) 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" id="form1">
  什么是你最喜欢的颜色？ <input type="text" name="fav_color"><br>
  <input type="submit">
</form>

<fieldset form="form1">
  Name: <input type="text" name="username"><br>
  Email: <input type="text" name="usermail"><br>
</fieldset>
```

### Input 示例

位于 HTML 表单之外的输入字段（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="form1">
  First name: <input type="text" name="fname"><br>
  <input type="submit" value="Submit">
</form>

Last name: <input type="text" name="lname" form="form1">
```

### Label 示例

位于表单外部的 [\<label>](../tags/label.md) 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="form1">
  <input type="radio" id="html" name="fav_language" value="HTML"><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form>

<label for="html">HTML</label>
```

### Meter 示例

位于表单外部的 [\<meter>](../tags/meter.md) 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" id="form1">
  First name: <input type="text" name="fname"><br>
  <input type="submit" value="Submit">
</form>

<meter form="form1" name="x1" min="0" low="40" high="90" max="100" value="95"></meter>
```

### Object 示例

位于表单外部的 [\<object>](../tags/object.md) 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="form1">
  First name: <input type="text" name="fname"><br>
  <input type="submit" value="Submit">
</form>

<object data="helloworld.swf" height="400" width="400" form="form1" name="obj1"></object>
```

### Output 示例

位于表单外部的 [\<output>](../tags/output.md) 元素（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="numform"
oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
  <input type="range" id="a" name="a" value="50">100
  +<input type="number" id="b" name="b" value="50">
  <br><br>
  <input type="submit">
</form>

<output form="numform" name="x" for="a b"></output>
```

### Select 示例

位于表单外部的下拉列表（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="carform">
  Firstname:<input type="text" name="fname">
  <input type="submit">
</form>

<select name="carlist" form="carform">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

### Textarea 示例

位于表单外部的文本区域（但仍然是表单的一部分）：

```html idoc:preview:iframe
<form action="/action_page.php" id="usrform">
  Name: <input type="text" name="usrname">
  <input type="submit">
</form>

<textarea name="comment" form="usrform">Enter text here...</textarea>
```

## 浏览器支持

`form` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| button   | 10.0          | ❌ 不支持 | 4.0           | 5.1           | 9.5           |
| fieldset | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
| input    | 9.0           | ❌ 不支持 | 4.0           | 5.1           | 10.6          |
| label    | Yes           | Yes           | Yes           | Yes           | Yes           |
| meter    | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
| object   | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
| output   | Yes           | ❌ 不支持 | Yes           | Yes           | Yes           |
| select   | Yes           | ❌ 不支持 | Yes           | Yes           | Yes           |
| textarea | Yes           | ❌ 不支持 | Yes           | Yes           | Yes           |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
