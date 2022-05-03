HTML charset 属性
===

## 定义和用法

当被 [`<meta>`](../tags/meta.md) 元素使用时，[charset](../tags/meta_charset.md) 属性指定 HTML 文档的字符编码。

当被 [`<script>`](../tags/script.md) 元素使用时，[charset](../tags/script_charset.md) 属性指定外部脚本文件中使用的字符编码。

HTML5 规范鼓励 Web 开发人员使用 UTF-8 字符集，它涵盖了世界上几乎所有的字符和符号！

## 适用于

`charset` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<meta>](../tags/meta.md)     | [charset](../tags/meta_charset.md)   |
| [\<script>](../tags/script.md) | [charset](../tags/script_charset.md) |

## 示例

### Meta 示例

指定 HTML 文档的字符编码：

```html
<head>
  <meta charset="UTF-8">
</head>
```

### Script 示例

带有 UTF-8 字符集的外部 JavaScript：

```html
<script src="myscripts.js" charset="UTF-8"></script>
```

## 浏览器支持

`charset` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<meta>](../tags/meta.md)     | Yes | Yes | Yes | Yes | Yes |
| [\<script>](../tags/script.md) | Yes | Yes | Yes | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg