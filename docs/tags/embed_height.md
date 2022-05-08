HTML \<embed> height 属性
===

## 示例

一张高宽均为 200 像素的图片：

```html idoc:preview:iframe
<embed
  src="../assets/editors-006.png"
  width="200"
  height="200"
>
```
<!--rehype:style=min-height: 200px;-->

## 定义和用法

`height` 属性指定嵌入内容的高度，以像素为单位。

**提示：** 使用 `width` 属性指定嵌入内容的宽度。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| height    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<embed height="pixels">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *pixels* | 嵌入内容的高度，以像素为单位（即 `height="100"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
