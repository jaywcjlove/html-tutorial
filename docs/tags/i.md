HTML \<i> 标签
===

## 示例

标记从文档中的普通的文本：

```html idoc:preview:iframe
<p>
HTML（<i>超文本标记语言</i>——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 <i>HTML</i> 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 <i>CSS</i>），或功能与行为（如 <i>JavaScript</i>）</p>
```
<!--rehype:style=min-height: 120px;-->

## 定义和用法

`<i>` 标签定义了文本的一部分以替代语音或语气。 里面的内容通常以*斜体*显示。

`<i>` 标签通常用于表示技术术语、来自另一种语言的短语、思想、船名等。

只有在没有更合适的语义元素时才使用 `<i>` 元素，例如：

* [\<em>](./em.md)（强调文本）
* [\<strong>](./strong.md)（重要文本）
* [\<mark>](./mark.md)（标签/突出显示的文本）
* [\<cite>](./cite.md)（作品的标题）
* [\<dfn>](./dfn.md)（定义术语）

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<i>    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<i>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。


## 事件属性

`<i>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<i>` 元素：

```css
i {
  font-style: italic;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg