HTML \<img> src 属性
===

## 示例

图像标记如下：

```html idoc:preview
<img src="../assets/chrome.svg">
```

## 定义和用法

必需的 `src` 属性指定图像的 URL。

有两种方法可以在 `src` 属性中指定 URL：

**① 绝对 URL** - 指向托管在另一个网站上的外部图像的链接。示例：`src="https://jaywcjlove.github.io/html-tutorial/assets/chrome.svg"`。

**注意 ⚠️：** 外部图像可能受版权保护。如果您没有获得使用许可，您可能违反了版权法。此外，您无法控制外部图像；它可以突然被删除或更改。

**② 相对 URL** - 链接到网站内托管的图像。此处，URL 不包含域名。如果 URL 开头没有斜杠，则它将相对于当前页面。示例：`src="chrome.svg"`。如果 URL 以斜杠开头，它将与域相关。示例：`src="/assets/chrome.svg"`。

**提示：** 几乎总是最好使用相对 URL。如果您更改域，它们不会中断。

**注意 ⚠️：** 如果浏览器找不到图像，则会显示断开的链接图标和 `alt` 文本。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| src       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img src="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 图片的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `src="http://www.example.com/image.gif"`） <br>* 相对 URL - 指向网站内的文件（如 `src="image.gif"`） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg