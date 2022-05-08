HTML \<button> name 属性
===

## 示例

两个具有相同 `name` 的按钮，在单击时提交不同的值：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  选择你最喜欢的主题：
  <button name="subject" type="submit" value="HTML">HTML</button>
  <button name="subject" type="submit" value="CSS">CSS</button>
</form>
```

## 定义和用法

`name` 属性指定 `<button>` 元素的名称。

`name` 属性用于在表单提交后引用表单数据，或引用 JavaScript 中的元素。

**提示：** 多个 `<button>` 元素可以共享相同的名称。 这允许您拥有多个具有相同名称的按钮，这些按钮在表单中使用时可以提交不同的值。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| name      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button name="name">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *name* | 按钮的名称 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg