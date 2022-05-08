HTML \<button> value 属性
===

## 示例

两个具有相同名称的按钮，在单击时提交不同的值：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  选择你最喜欢的主题：
  <button name="subject" type="submit" value="fav_HTML">HTML</button>
  <button name="subject" type="submit" value="fav_CSS">CSS</button>
</form>
```

## 定义和用法

`value` 属性指定 HTML 表单中 `<button>` 的初始值。

**注意：** 在表单中，仅当使用按钮本身提交表单时，才会提交按钮及其值。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| value     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** 如果您在 HTML 表单中使用 `<button>` 元素，Internet Explorer 8 之前的版本将提交 `<button>` 和 `</button>` 标签之间的文本，而 其他浏览器将提交 `value` 属性的内容。

## 语法

```html
<button value="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *value* | 按钮的初始值 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
