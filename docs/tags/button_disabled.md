HTML \<button> disabled 标签
===

## 示例

禁用的按钮：

```html idoc:preview:iframe
<button type="button" disabled>Click Me!</button>
```

## 定义和用法

`disabled` 属性是一个布尔属性。

如果存在，它指定应该禁用该按钮。

禁用的按钮不可用且不可点击。

`disabled` 属性可以设置为阻止用户点击按钮，直到满足其他条件（如选择复选框等）。 然后，JavaScript 可以删除禁用的值，并使按钮再次可点击。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| disabled  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button disabled>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg