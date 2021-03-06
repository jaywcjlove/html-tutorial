HTML \<tbody> 标签
===

## 示例

带有 \<thead>、\<tbody> 和 \<tfoot> 元素的 HTML 表格：

```html idoc:preview:iframe
<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
    </tr>
  </tfoot>
</table>
```
<!--rehype:style=height: 150px;-->

## 定义和用法

`<tbody>` 标签用于对 HTML 表格中的正文内容进行分组。

`<tbody>` 元素与 [\<thead>](./thead.md) 和 [\<tfoot>](./tfoot.md) 元素一起使用来指定表格的每个部分（正文、页眉、页脚）。

浏览器可以使用这些元素来启用独立于页眉和页脚的表格正文滚动。此外，当打印跨多页的大表格时，这些元素可以使表格页眉和页脚打印在每页的顶部和底部。

**注意：** `<tbody>` 元素内部必须有一个或多个 [\<tr>](./tr.md) 标签。

`<tbody>` 标签必须在以下上下文中使用：作为 [\<table>](./table.md) 元素的子元素，在任何 [\<caption>](./caption.md) 之后，[\< colgroup>](./colgroup.md) 和 [\<thead>](./thead.md) 元素。

**提示：** \<thead>、`<tbody>` 和 \<tfoot> 元素默认不会影响表格的布局。但是，您可以使用 CSS 来设置这些元素的样式（参见下面的示例）！

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<tbody> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<tbody>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<tbody>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 样式化 \<thead>、\<tbody> 和 \<tfoot>：

```html idoc:preview:iframe
<html>
<head>
  <style>
    thead {color: green;}
    tbody {color: blue;}
    tfoot {color: red;}
    table, th, td {
      border: 1px solid black;
    }
  </style>
</head>
<body>
<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
    </tr>
  </tfoot>
</table>
```
<!--rehype:style=height: 140px;-->

如何对齐 \<tbody> 中的内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:100%">
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody style="text-align:right">
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
</table>
```
<!--rehype:style=height: 130px;-->

如何垂直对齐 \<tbody> 内的内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:50%;">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tbody style="vertical-align:bottom">
    <tr style="height:100px">
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr style="height:100px">
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
</table>
```
<!--rehype:style=height: 280px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<tbody>` 元素：

```css
tbody {
  display: table-row-group;
  vertical-align: middle;
  border-color: inherit;
}
```



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg