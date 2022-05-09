HTML contenteditable 属性
===

## 定义和用法

`contenteditable` 属性指定元素的内容是否可编辑。

**注意：** 当一个元素没有设置 `contenteditable` 属性时，该元素会从其父元素继承它。

## 适用于

`contenteditable` 属性是一个 [全局属性](../reference/standardattributes.md)，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 所有 [HTML](../tags/README.md) 元素 | [contenteditable](./global/contenteditable.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

可编辑的段落：

```html idoc:preview:iframe
<p contenteditable="true" autofocus>这是一个可编辑的段落。</p>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| contenteditable | 4.0 | 6.0 | 3.5 | 3.1 | 10.1 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
