HTML colspan 属性
===

## 定义和用法

`colspan` 属性定义了一个表格单元格应该跨越的列数。

## 适用于

`colspan` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<td>](../tags/td.md) | [colspan](../tags/td_colspan.md) |
| [\<th>](../tags/th.md) | [colspan](../tags/th_colspan.md) |

## 示例

### Td 示例

一个包含跨两列的表格单元格的 HTML 表格：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; border-collapse: collapse; }
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
    <td>$100</td>
  </tr>
  <tr>
    <td colspan="2">Sum: $180</td>
  </tr>
</table>
```
<!--rehype:style=height: 150px;-->

### Th 示例

一个包含跨两列的标题单元格的 HTML 表格：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; border-collapse: collapse; }
</style>
<table>
  <tr>
    <th colspan="2">Monthly Savings</th>
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

## 浏览器支持

`colspan` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<td>](../tags/td.md) | Yes | Yes | Yes | Yes | Yes |
| [\<th>](../tags/th.md) | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
