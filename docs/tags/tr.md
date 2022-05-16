HTML \<tr> 标签
===

## 示例

一个简单的三行 HTML 表格； 一个标题行和两个数据行：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
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
```
<!--rehype:style=height: 110px;-->

## 定义和用法

`<tr>` 标签定义 HTML 表格中的一行。

`<tr>` 元素包含一个或多个 [\<th>](./th.md) 或 [\<td>](./td.md) 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<tr>   | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<tr>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<tr>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

如何对齐 \<tr> 中的内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:100%">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr style="text-align:right">
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

如何将背景颜色添加到表格行（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table>
  <tr style="background-color:#FF0000">
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

如何在 \<tr> 中垂直对齐内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="height:200px">
  <tr  style="vertical-align:top">
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr style="vertical-align:bottom">
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```

如何创建表头：

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
  </tr>
</table>
```
<!--rehype:style=height: 160px;-->

如何创建带有标题的表格：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
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
<!--rehype:style=height: 130px;-->

## 相关页面

HTML 教程: [HTML Tables](../tutorial/tables.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<tr>` 元素：

```css
tr {
  display: table-row;
  vertical-align: inherit;
  border-color: inherit;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg