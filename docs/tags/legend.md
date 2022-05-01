HTML \<legend> 标签
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

`<legend>` 标记定义了 [\<fieldset>](./fieldset.md) 元素的标题。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<legend>  | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<ins>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<ins>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

让字段集标题向右浮动（使用 CSS）：

```html idoc:preview:iframe
<form action="/action_page.php">
  <fieldset>
    <legend style="float:right">Personalia:</legend>
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

使用 CSS 设置 [\<fieldset>](./fieldset.md) 和 \<legend> 的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    fieldset {
      background-color: #eeeeee;
    }
    legend {
      background-color: gray;
      color: white;
      padding: 5px 10px;
    }
    input {
      margin: 5px;
    }
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
<!--rehype:style=height: 330px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<legend>` 元素：

```css
legend {
  display: block;
  padding-left: 2px;
  padding-right: 2px;
  border: none;
}
```
