HTML \<a> download 标签
===

## 示例

单击链接时下载文件（而不是导航到文件）：

```html idoc:preview:iframe
<a href="../assets/edge.svg" download>
  下载 edge.svg 图标
</a>
```

## 定义和用法

`download` 属性指定当用户单击超链接时将下载目标（[`href`](./a_href.md) 属性中指定的文件）。

`download` 属性的可选值将是文件下载后的新名称。 对允许值没有限制，浏览器会自动检测正确的文件扩展名并将其添加到文件中（.img、.pdf、.txt、.html 等）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| download  | 14.0\* | 18.0 | 20.0\* | 10.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

\* Chrome 65+ 和 Firefox 仅支持同源下载链接。

## 语法

```html
<a download="filename">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| *filename* | 可选的。 指定下载文件的新文件名 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

为下载属性指定一个值，它将是下载文件的新文件名（“chrome.svg”而不是“edge.svg”）：

```html idoc:preview:iframe
<a href="../assets/edge.svg" download="chrome">
  下载 svg 图标
</a>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg