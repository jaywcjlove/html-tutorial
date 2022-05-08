HTML \<del> cite 属性
===

## 示例

已删除的文本，带有一个文档的 URL，该文档解释了该文本被删除的原因：

```html idoc:preview:iframe
<p><del cite="del.html">此文字已被删除</del></p>
```

## 定义和用法

`cite` 属性指定了一个文档的 URL，该文档解释了删除文本的原因。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| cite      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** `cite` 属性在普通网络浏览器中没有视觉效果，但可以被屏幕阅读器使用。

## 语法

```html
<del cite="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定解释文本被删除原因的文档地址。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `cite="http://www.example.com/page.htm"`） <br>* 相对 URL - 指向网站内的页面（如 `cite="page.htm"`） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
