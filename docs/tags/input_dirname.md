HTML \<input> dirname 属性
===

## 示例

将提交字段文本方向的 HTML 表单：

```html
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname" dirname="fname.dir">
  <input type="submit" value="Submit">
</form>
```

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname" dirname="fname.dir">
  <input type="submit" value="Submit">
</form>
当表单被提交时，输入字段的文本方向也会被提交。<br>
结果示例：fname=wwwww&fname.dir=ltr 
```

## 定义和用法

`dirname` 属性启用输入字段的文本方向的提交

`dirname` 属性的值始终是输入字段的名称，后跟 `.dir`。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| dirname   | Yes | 79.0 | ❌ 不支持 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input name="myname" dirname="myname.dir">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *name*.dir | 指定将提交输入字段的文本方向。 |
<!--rehype:style=width: 100%; display: inline-table;-->


[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
