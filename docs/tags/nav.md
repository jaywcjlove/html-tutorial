HTML \<nav> Tag
===

## 示例

一组导航链接：

```html idoc:preview:iframe
<nav>
  <a href="../reference/byfunc.html">HTML 标签参考</a> |
  <a href="../reference/standardattributes.html">全局属性</a> |
  <a href="../reference/eventattributes.html">事件属性</a> |
  <a href="../reference/charactersets_entities.html">Python</a>
</nav>
```

## 定义和用法

`<nav>` 标签定义了一组导航链接。

请注意，并非文档的所有链接都应该在 `<nav>` 元素内。 `<nav>` 元素仅用于主要的导航链接块。

浏览器，例如残疾用户的屏幕阅读器，可以使用此元素来确定是否省略此内容的初始呈现。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<nav>  | 5.0 | 9.0 | 4.0 | 5.0 | 11.1 |

## 全局属性

`<nav>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<nav>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<menu>` 元素：

```css
nav {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg