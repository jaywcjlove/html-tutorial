HTML \<img> alt 属性
===

## 示例

指定替代文本的图像，下图图片不存在显示 `alt` 中的文本内容：

```html idoc:preview
<img src="../assets/editors-001xxx.png" alt="这是一个截图" width="500" height="600">
```
<!--rehype:style=min-height: 120px;-->

## 定义和用法

如果图像无法显示，则必需的 `alt` 属性指定图像的替代文本。

如果用户由于某种原因无法查看图像（由于连接速度慢、`src` 属性中的错误或用户使用屏幕阅读器），`alt` 属性会为图像提供替代信息。

**提示：** 要为图像创建工具提示，请使用 `title` 属性！

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| alt       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img alt="text">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *text* | 指定图像的替代文本。替代文本的准则：<br>* 如果图像包含信息，则文本应描述图像 <br>* 如果图像在 \<a> 元素内，文本应说明链接的位置 <br>* 如果图像仅用于装饰，请使用 `alt=""` |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg