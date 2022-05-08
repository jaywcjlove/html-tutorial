HTML \<iframe> src 属性
===

## 示例

一个 \<iframe> 最简单的用法：

```html idoc:preview
<iframe src="./html.html" title="HTML Tutorial" height="100%" width="100%"></iframe>
```
<!--rehype:style=min-height: 260px;-->

## 定义和用法

`src` 属性指定要嵌入 iframe 的文档的地址。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| src       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<iframe src="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定要嵌入 iframe 的文档的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `src="http://www.example.com/default.htm"`） <br>* 相对 URL - 指向网站内的文件（如 `src="default.htm"`） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

