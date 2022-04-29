HTML \<figure> Tag
===

## 示例

使用 \<figure> 元素标记文档中的照片，并使用 [\<figcaption>](./figcaption.md) 元素定义照片的标题：

```html idoc:preview
<figure>
  <img src="../assets/editors-006.png" alt="Trulli" height="120">
  <figcaption>图.1 - 第一个HTML页面</figcaption>
</figure>
```
<!--rehype:style=min-height: 200px;-->

## 定义和用法

`<figure>` 标签指定了独立的内容，如插图、图表、照片、代码列表等。

`<figure>` 元素的内容与主流程相关，但它的位置与主流程无关，如果移除它不应该影响文档的流程。

**提示：** [\<figcaption>](./figcaption.md) 元素用于为 `<figure>` 元素添加标题。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<figure> | 8.0 | 9.0 | 4.0 | 5.1 | 11.0 |

## 全局属性

`<figure>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<figure>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<figure> 和 [\<figcaption>](./figcaption.md) 的样式：

```html idoc:preview:iframe
<html>
<head>
<style>
figure { border: 1px #cccccc solid; padding: 4px; margin: auto; }
figcaption {
  background-color: black;
  color: white;
  font-style: italic;
  padding: 2px;
  text-align: center;
}
</style>
</head>
<body>
  <figure>
    <img src="../assets/editors-006.png" alt="Trulli" height="230">
    <figcaption>图.1 - 第一个HTML页面</figcaption>
  </figure>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<figure>` 元素：

```css
figure {
  display: block;
  margin-top: 1em;
  margin-bottom: 1em;
  margin-left: 40px;
  margin-right: 40px;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg