HTML \<img> height 属性
===

## 示例

一个高度为 600 像素，宽度为 500 像素的图像：

```html idoc:preview
<img src="../assets/chrome.svg" width="500" height="600">
```
<!--rehype:style=min-height: 620px;-->

## 定义和用法

`height` 属性指定图像的高度，以像素为单位。

**提示：** 始终为图像指定 `height` 和 `width` 属性。 如果设置了高度和宽度，则在加载页面时保留图像所需的空间。 但是，如果没有这些属性，浏览器将不知道图像的大小，也无法为其预留适当的空间。 效果将是页面布局将在加载期间更改（同时加载图像）。

**提示：** 使用 `height` 和 `width` 属性缩小大图会强制用户下载大图（即使它在页面上看起来很小）。 为避免这种情况，请在将图像用于页面之前使用程序重新缩放图像。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| height    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img height="pixels">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *pixels* | 以像素为单位的高度（例如 `height="100"`） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg