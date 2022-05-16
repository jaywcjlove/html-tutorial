HTML \<table> 标签
===

## 示例

一个简单的 HTML 表格，包含两列和两行：

```html idoc:preview:iframe
<table>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

## 定义和用法

`<table>` 标签定义了一个 HTML 表格。

一个 HTML 表格由一个 `<table>` 元素和一个或多个 [\<tr>](./tr.md)、[\<th>](./th.md) 和 [\<td>](./td.md) 元素。

\<tr> 元素定义表格行，\<th> 元素定义表格标题，\<td> 元素定义表格单元格。

HTML 表格还可以包括 [\<caption>](./caption.md)、[\<colgroup>](./colgroup.md)、[\<thead>](./thead.md)、[\<tfoot>](./tfoot.md) 和 [\<tbody>](./tbody.md) 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<table> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<table>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<table>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

如何向表格添加折叠边框（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    table, th, td {
      border: 1px solid black;
      border-collapse: collapse;
    }
  </style>
</head>
<body>
  <table>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </table>
</body>
</html>
```
<!--rehype:style=height: 150px;-->

如何右对齐表格（使用 CSS）：

```html idoc:preview:iframe
<table style="float:right">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何居中对齐表格（使用 CSS）

```html idoc:preview:iframe
<style>
  table, th, td {
    border: 1px solid black;
  }
  table.center {
    margin-left: auto;
    margin-right: auto;
  }
</style>
<table class="center">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何向表格添加背景颜色（使用 CSS）：

```html idoc:preview:iframe
<table style="background-color:#00FF00">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何向表格添加填充（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    table, th, td {
      border: 1px solid black;
    }
    th, td {
      padding: 10px;
    }
  </style>
</head>
<body>
  <table>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </table>
</body>
</html>
```
<!--rehype:style=height: 210px;-->

如何设置表格宽度（使用 CSS）：

```html idoc:preview:iframe
<table style="width:400px">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何创建表头：

```html idoc:preview:iframe
<style>
  table, th, td {
    border: 1px solid black;
  }
</style>
<table>
  <tr>
    <th>姓名</th>
    <th>邮箱</th>
    <th>电话</th>
  </tr>
  <tr>
    <td>周杰伦</td>
    <td>zhou@example.com</td>
    <td>123-45-678</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

如何创建带有标题的表格：

```html idoc:preview:iframe
<style>
  table, th, td {
    border: 1px solid black;
  }
</style>
<table>
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 160px;-->

如何定义跨越多于一行或一列的表格单元格：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table>
  <tr>
    <th>姓名</th>
    <th>邮箱</th>
    <th colspan="2">电话</th>
  </tr>
  <tr>
    <td>周杰伦</td>
    <td>zhou@example.com</td>
    <td>123-45-678</td>
    <td>021-00-546</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

## 相关页面

HTML 教程: [HTML Tables](../tutorial/tables.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<table>` 元素：

```css
table {
  display: table;
  border-collapse: separate;
  border-spacing: 2px;
  border-color: gray;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg