HTML \<colgroup> span 属性
===

## 示例

使用 \<colgroup> span 属性设置前两列的背景颜色：

```html idoc:preview
<table>
  <colgroup span="2" style="background:red"></colgroup>
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
  <tr>
    <td>5869207</td>
    <td>My first CSS</td>
    <td>$49</td>
  </tr>
</table>
```

## 定义和用法

`span` 属性定义了 `<colgroup>` 元素应该跨越的列数。

**提示：** 要为 `<colgroup>` 中的列定义不同的属性，请使用 `<colgroup>` 标记中的 `<col>` 标记。

## 浏览器支持

| Attribute  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| span      | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<colgroup span="*number*">
```

## 属性值

| 值 Value | 描述 Description |
| -------- | ------ |
| *number* | 设置列组应跨越的列数 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg