HTML \<div> Tag
===

## 示例

文档中使用 CSS 设置样式的 \<div> 部分：

```html idoc:preview:iframe
<html>
<head>
<style>
  .myDiv { border: 5px outset red; background-color: lightblue; text-align: center; }
</style>
</head>
<body>
  <div class="myDiv">
    <h2>这是 div 元素中的标题</h2>
    <p>这是 div 元素中的一些文本。</p>
  </div>
</body>
</html>
```

## 定义和用法

`<div>` 标签定义 HTML 文档中的一个分区或一个部分。

`<div>` 标签用作 HTML 元素的容器 - 然后使用 CSS 设置样式或使用 JavaScript 进行操作。

`<div>` 标签很容易通过使用 class 或 id 属性来设置样式。

任何类型的内容都可以放在`<div>`标签内！

**注意：** 默认情况下，浏览器总是在 `<div>` 元素前后放置一个换行符。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<div>  | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<div>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<div>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML tutorial: [HTML Block and Inline Elements](../tutorial/blocks.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<div>` 元素：

```css
div {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg