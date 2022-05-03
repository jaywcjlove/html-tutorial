HTML cite 属性
===

## 定义和用法

`cite` 属性指定了一个文档的 URL，该文档解释了引用，或者为什么插入/更改了文本。

## 适用于

`cite` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<blockquote>](../tags/blockquote.md) | [cite](../tags/blockquote_cite.md) |
| [\<del>](../tags/del.md)               | [cite](../tags/del_cite.md)        |
| [\<ins>](../tags/ins.md)               | [cite](../tags/ins_cite.md)        |
| [\<q>](../tags/q.md)                   | [cite](../tags/q_cite.md)          |

## 示例

### Blockquote 示例

从另一个来源引用的部分：

```html idoc:preview:iframe
<blockquote cite="https://github.com/jaywcjlove/html-tutorial">

HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）。

</blockquote>
```

### Del 示例

已删除的文本，带有一个文档的 URL，该文档解释了该文本被删除的原因：

```html idoc:preview:iframe
<p>
  <del cite="../tags/del.html">此文字已被删除</del>
</p>
```

### Ins 示例

一个插入的文本，带有一个文档的 URL，解释了为什么插入文本：

```html idoc:preview:iframe
<p>
  这是一个文本。
  <ins cite="../tags/ins.html">这是插入的文本。</ins>
</p>
```

### Q 示例

指定报价的来源 URL：

```html idoc:preview:iframe
<p>超文本标记语言
<q cite="https://github.com/jaywcjlove/html-tutorial">
  HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。
</p>
```

## 浏览器支持

`cite` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [blockquote](../tags/blockquote.md) | Yes | Yes | Yes | Yes | Yes |
| [del](../tags/del.md)               | Yes | Yes | Yes | Yes | Yes |
| [ins](../tags/ins.md)               | Yes | Yes | Yes | Yes | Yes |
| [q](../tags/q.md)                   | Yes | Yes | Yes | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
