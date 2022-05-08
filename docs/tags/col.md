HTML \<col> 标签
===

## 示例

使用 \<colgroup> 和 \<col> 标签设置三列的背景颜色：

```html idoc:preview
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

`<col>` 标记为 [\<colgroup>](./colgroup.md) 元素中的每一列指定列属性。

`<col>` 标签可用于将样式应用于整个列，而不是为每个单元格、每一行重复样式。

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<col>  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| [span](./col_span.md) | *number* | 指定 \<col> 元素应跨越的列数 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<col>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<col>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

对齐表格列中的文本（使用 CSS）：

```html idoc:preview
<table style="width:100%">
  <tr>
    <th>ISBN</th>
    <th>Title</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>3476896</td>
    <td>My first HTML</td>
    <td style="text-align:right">$53</td>
  </tr>
  <tr>
    <td>2489604</td>
    <td>My first CSS</td>
    <td style="text-align:right">$47</td>
  </tr>
</table>
```

表格列中的垂直对齐文本（使用 CSS）：

```html idoc:preview
<table style="height:200px">
  <tr>
    <th>Month</th>
    <th style="vertical-align:bottom">Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td style="vertical-align:bottom">$100</td>
  </tr>
</table>
```

指定表格列的宽度（使用 CSS）：

```html idoc:preview
<table>
  <tr>
    <th style="width:130px">Month</th>
    <th style="width:80px">Savings</th>
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

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<col>` 元素：

```css
col {
  display: table-column;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg