HTML \<fieldset> 标签
===

## 示例

对表单中的相关元素进行分组：

```html idoc:preview:iframe
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br><br>
    <label for="birthday">Birthday:</label>
    <input type="date" id="birthday" name="birthday"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

## 定义和用法

`<fieldset>` 标签用于对表单中的相关元素进行分组。

`<fieldset>` 标签在相关元素周围绘制了一个框。

## 提示和注意事项

**提示：** [\<legend>](./legend.md) 标签用于定义 `<fieldset>` 元素的标题。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<fieldset> | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| [disabled](./fieldset_disabled.md) | disabled   | 指定应该禁用一组相关的表单元素 |
| [form](./fieldset_form.md) | *form\_id* | 指定字段集属于哪个表单 |
| [name](./fieldset_name.md) | *text*     | 指定字段集的名称 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<fieldset>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<fieldset>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<fieldset> 和 [\<legend>](./legend.md) 的样式：

```html idoc:preview
<html>
<head>
  <style>
    fieldset { background-color: #eeeeee; }
    legend {
      background-color: gray;
      color: white;
      padding: 5px 10px;
    }
    input { margin: 5px; }
  </style>
</head>
<body>
  <form action="/action_page.php">
    <fieldset>
      <legend>Personalia:</legend>
      <label for="fname">First name:</label>
      <input type="text" id="fname" name="fname"><br><br>
      <label for="lname">Last name:</label>
      <input type="text" id="lname" name="lname"><br><br>
      <label for="email">Email:</label>
      <input type="email" id="email" name="email"><br><br>
      <label for="birthday">Birthday:</label>
      <input type="date" id="birthday" name="birthday"><br><br>
      <input type="submit" value="Submit">
    </fieldset>
  </form>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<fieldset>` 元素：

```css
fieldset {
  display: block;
  margin-left: 2px;
  margin-right: 2px;
  padding-top: 0.35em;
  padding-bottom: 0.625em;
  padding-left: 0.75em;
  padding-right: 0.75em;
  border: 2px groove (*internal value*);
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg