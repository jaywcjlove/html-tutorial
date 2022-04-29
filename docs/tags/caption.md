HTML \<caption> Tag
===

## 示例

带标题的表格：

```html idoc:preview
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
</table>
```

## 定义和用法

`<caption>` 标签定义了一个表格标题。

`<caption>` 标记必须紧跟在 [\<table>](./table.md) 标记之后。

**提示：** 默认情况下，表格标题将在表格上方居中对齐。 但是，CSS 属性 `text-align` 和 `caption-side` 可用于对齐和放置标题。

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<caption> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<button>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<button>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

位置表标题（使用 CSS）：

```html idoc:preview
<table>
  <caption style="text-align:right">My savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
<br>

<table>
  <caption style="caption-side:bottom">My savings</caption>
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

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<caption>` 元素：

```css
caption {
  display: table-caption;
  text-align: center;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg