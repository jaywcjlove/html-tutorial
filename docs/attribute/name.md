HTML name 属性
===

## 定义和用法

`name` 属性指定 HTML 元素的名称。

这个 `name` 属性可用于引用 JavaScript 中的元素。

对于 [\<form>](../tags/form.md) 元素，`name` 属性在提交数据时用作参考。

对于 [\<iframe>](../tags/iframe.md) 元素，`name` 属性可用于定位表单提交。

对于 [\<map>](../tags/map.md) 元素，`name` 属性与 [`<img>`](../tags/img.md) 的[`usemap`](./usemap.md) 属性相关联，并在图像和地图之间创建关系。

对于 [\<meta>](../tags/meta.md) 元素，`name` 属性指定了 [`content`](./content.md) 属性的信息/值的名称。

对于 [\<param>](../tags/param.md) 元素，`name` 属性与 [`value`](./value.md) 属性一起使用，以指定使用 [\<object>](../tags/object.md) 标签指定的插件的参数。

## 定义和用法

The `name` attribute can be used on the following elements:

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<button>](../tags/button.md)     | [name](../tags/button_name.md)   |
| [\<fieldset>](../tags/fieldset.md) | [name](../tags/fieldset_name.md) |
| [\<form>](../tags/form.md)         | [name](../tags/form_name.md)     |
| [\<iframe>](../tags/iframe.md)     | [name](../tags/iframe_name.md)   |
| [\<input>](../tags/input.md)       | [name](../tags/input_name.md)    |
| [\<map>](../tags/map.md)           | [name](../tags/map_name.md)      |
| [\<meta>](../tags/meta.md)         | [name](../tags/meta_name.md)     |
| [\<object>](../tags/object.md)     | [name](../tags/object_name.md)   |
| [\<output>](../tags/output.md)     | [name](../tags/output_name.md)   |
| [\<param>](../tags/param.md)       | [name](../tags/param_name.md)    |
| [\<select>](../tags/select.md)     | [name](../tags/select_name.md)   |
| [\<textarea>](../tags/textarea.md) | [name](../tags/textarea_name.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### 示例

两个具有相同名称的按钮，在单击时提交不同的值：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  Choose your favorite subject:
  <button name="subject" type="submit" value="HTML">HTML</button>
  <button name="subject" type="submit" value="CSS">CSS</button>
</form>
```

### Fieldset 示例

具有 name 属性的 \<fieldset>：

```html idoc:preview:iframe
<fieldset name="personalia">
  Name: <input type="text"><br>
  Email: <input type="text"><br>
</fieldset>
```

### Form 示例

具有 name 属性的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php" method="get" name="myForm">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="button" onclick="formSubmit()" value="Send form data!">
</form>
```

### Iframe 示例

用作链接目标的 \<iframe>：

```html idoc:preview:iframe
<iframe src="./max.html" name="iframe_a"></iframe>
<br/>
<a href="../tags/iframe.html" target="iframe_a">点击在 iframe 中打开</a>
```
<!--rehype:style=min-height: 260px;-->

### Input 示例

具有三个输入字段的 HTML 表单； 两个文本字段和一个提交按钮：

```html idoc:preview:iframe
<form action="/action_page.php">
  Name: <input type="text" name="fullname"><br>
  Email: <input type="text" name="email"><br>
  <input type="submit" value="Submit">
</form>
```

### Map 示例

带有可点击区域的图像 [\<map>](../tags/map.md)：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
</map>
```

### Meta 示例

使用 name 属性来定义 HTML 文档的描述、关键字和作者：

```html
<head>
  <meta name="description" content="Free Web tutorials">
  <meta name="keywords" content="HTML,CSS,JavaScript">
  <meta name="author" content="Hege Refsnes">
</head>
```

### Object 示例

具有 name 属性的 [\<object>](../tags/object.md) 元素：

```html idoc:preview:iframe
<object
  data="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4"
  height="200"
  name="obj1">
</object>
```
<!--rehype:style=min-height: 220px;-->

### Output 示例

执行计算并在 \<output> 元素中显示结果：

```html idoc:preview:iframe
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
  <input type="range" id="a" value="50">100
  +<input type="number" id="b" value="50">
  =<output name="x" for="a b"></output>
</form>
```

### Param 示例

将“autoplay”参数设置为“true”，这样声音就会在页面加载后立即开始播放：

```html idoc:preview:iframe
<object data="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <param name="autoplay" value="true">
</object>
```
<!--rehype:style=min-height: 220px;-->

### Select 示例

带有名称属性的下拉列表：

```html idoc:preview:iframe
<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

### Textarea 示例

具有名称属性的文本区域：

```html idoc:preview:iframe
<form action="/action_page.php">
  <textarea name="comment">在这里输入文本...</textarea>
  <input type="submit">
</form>
```

## 浏览器支持

`multiple` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| button   | Yes  | Yes           | Yes | Yes  | Yes  |
| fieldset | Yes  | ❌ 不支持 | Yes | Yes  | Yes  |
| form     | Yes  | Yes           | Yes | Yes  | Yes  |
| iframe   | Yes  | Yes           | Yes | Yes  | Yes  |
| input    | 1.0  | 2.0           | 1.0 | 1.0  | 1.0  |
| map      | Yes  | Yes           | Yes | Yes  | Yes  |
| meta     | Yes  | Yes           | Yes | Yes  | Yes  |
| object   | Yes  | Yes           | Yes | Yes  | Yes  |
| output   | 10.0 | ❌ 不支持 | 4.0 | 5.1  | 11.0 |
| param    | Yes  | Yes           | Yes | Yes  | Yes  |
| select   | Yes  | Yes           | Yes | Yes  | Yes  |
| textarea | Yes  | Yes           | Yes | Yes  | Yes  |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg