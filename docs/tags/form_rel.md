HTML \<form> rel 属性
===

## 定义和用法

`rel` 属性指定当前文档和链接文档之间的关系。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| rel       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form rel="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| external   | 指定引用的文档不是当前站点的一部分 |
| help       | 帮助文档的链接 |
| license    | 文档版权信息的链接 |
| next       | 选择中的下一个文档 |
| nofollow   | 指向未经认可的文档的链接，例如付费链接。 （Google 使用“nofollow”来指定 Google 搜索蜘蛛不应跟随该链接） |
| noopener   | |
| noreferrer | 指定如果用户点击超链接，浏览器不应该发送 HTTP 引用标头 |
| opener     | |
| prev       | 选择中的上一个文档 |
| search     | 指向文档搜索工具的链接 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

