HTML \<abbr> 标签
===

## 实例

标记一个缩写：

```html idoc:preview
The <abbr title="People's Republic of China">PRC</abbr> was founded in 1949.
```

## 定义和用法

`<abbr>` 标签定义缩写或首字母缩略词，如 `HTML`, `CSS`, `Mr.`, `Dr.`, `ASAP`, `ATM`。

提示：当您将鼠标悬停在元素上时，使用全局标题属性显示缩写/首字母缩略词的描述。

## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;abbr&gt;__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<abbr>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<abbr>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

`<abbr>` 也可以与 [\<dfn>](./dfn.md) 一起使用来定义缩写：

```html idoc:preview
<p><dfn><abbr title="Cascading Style Sheets">CSS</abbr>
</dfn> is a language that describes the style of an HTML document.</p>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<abbr>` 元素：

```css
abbr {
  display: inline;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg