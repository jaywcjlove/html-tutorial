HTML headers 属性
===

## 定义和用法

`headers` 属性指定一个或多个与表格单元格相关的标题单元格。

## 适用于

`headers` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<td>](../tags/td.md) | [headers](../tags/td_headers.md) |
| [\<th>](../tags/th.md) | [headers](../tags/th_headers.md) |

## 示例

### Td 示例

指定每个 [\<td>](../tags/td.md) 元素相关的 [\<th>](../tags/th.md) 元素：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
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

### Th 示例

指定每个标题单元格相关的 [\<th>](../tags/th.md) 元素：

```html idoc:preview:iframe
<style>
  table, th, td { border: 1px solid black; }
</style>
<table>
  <tr>
    <th id="name" colspan="2">姓名</th>
  </tr>
  <tr>
    <th headers="name">名</th>
    <th headers="name">姓</th>
  </tr>
</table>
```
<!--rehype:style=height: 110px;-->

## 浏览器支持

`headers` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<td>](../tags/td.md) | Yes | Yes | Yes | Yes | Yes |
| [\<th>](../tags/th.md) | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
