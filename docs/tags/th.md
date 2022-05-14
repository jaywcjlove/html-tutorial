HTML \<th> Tag
===

## 示例

一个包含三行、两个标题单元格和四个数据单元格的简单 HTML 表格：

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

`<th>` 标签定义 HTML 表格中的标题单元格。

HTML 表格有两种单元格：

* 标题单元格 - 包含标题信息（使用 `<th>` 元素创建）
* 数据单元格 - 包含数据（使用 [\<td>](./td.md) 元素创建）

`<th>` 元素中的文本默认为粗体并居中。

\<td> 元素中的文本默认为常规且左对齐。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<th>   | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [abbr](./th_abbr.md)       | *text*                    | 指定标题单元格中内容的缩写版本 |
| [colspan](./th_colspan.md) | *number*                  | 指定标题单元格应跨越的列数 |
| [headers](./th_headers.md) | *header\_id*              | 指定一个或多个与单元格相关的标题单元格 |
| [rowspan](./th_rowspan.md) | *number*                  | 指定标题单元格应跨越的行数 |
| [scope](./th_scope.md)     | col colgroup row rowgroup | 指定标题单元格是否是列、行或列或行组的标题 |

## 全局属性

`<th>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<th>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

如何对齐 \<td> 中的内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:100%">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td style="text-align:right">$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td style="text-align:right">$80</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何向表格单元格添加背景颜色（使用 CSS）：

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
    <td style="background-color:#FF0000">January</td>
    <td style="background-color:#00FF00">$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何设置表格单元格的高度（使用 CSS）：

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
    <td style="height:100px">January</td>
    <td style="height:100px">$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何在表格单元格中指定不换行（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table>
  <tr>
    <th>Poem</th>
  </tr>
  <tr>
    <td style="white-space:nowrap">Never increase, beyond what is necessary, the number of entities required to explain anything</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

如何垂直对齐 \<td> 中的内容（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:50%;">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr style="height:100px">
    <td style="vertical-align:bottom">January</td>
    <td style="vertical-align:bottom">$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

如何设置表格单元格的宽度（使用 CSS）：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table style="width:100%">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td style="width:70%">January</td>
    <td style="width:30%">$100</td>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

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

大多数浏览器将显示具有以下默认值的 `<th>` 元素：

```css
th {
  display: table-cell;
  vertical-align: inherit;
  font-weight: bold;
  text-align: center;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg