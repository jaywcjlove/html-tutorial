HTML \<col> span 属性
===

## 示例

在这里，前两列的背景色应该是红色：

```html idoc:preview:iframe
<table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>ISBN</th>
    <th>Title</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>3476896</td>
    <td>My first HTML</td>
    <td>$53</td>
  </tr>
</table>
```

## 定义和用法

`span` 属性定义了 `<col>` 元素应该跨越的列数。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| span      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<col span="number">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | 设置 \<col> 元素应跨越的列数 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
