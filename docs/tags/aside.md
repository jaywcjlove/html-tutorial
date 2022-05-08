HTML \<aside> 标签
===

## 示例

显示除了它所在的内容之外的一些内容：

```html idoc:preview:iframe
<p>今年夏天，我和我的家人参观了 未来世界中心。 天气很好，Epcot 很棒！ 我和家人一起度过了一个美好的夏天！</p>
<aside>
  <h4>未来世界中心</h4>
  <p>HTML的全称为超文本标记语言，是一种标记语言。它包括一系列标签．通过这些标签可以将网络上的文档格式统一，使分散的 Internet 资源连接为一个逻辑整体。</p>
</aside>
```

## 定义和用法

`<aside>` 标签定义了除了它所在的内容之外的一些内容。

旁白内容应与周围内容间接相关。

**提示：** `<aside>` 内容通常作为侧边栏放置在文档中。

**注意：** `<aside>` 元素在浏览器中不会呈现为任何特殊内容。 但是，您可以使用 CSS 来设置 `<aside> `元素的样式（参见下面的示例）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | ---- |
| \<aside> | 6.0 | 9.0 | 4.0 | 5.0 | 11.1 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<aside>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<aside>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<aside> 元素的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    aside { width: 30%; padding-left: 15px; margin-left: 15px; float: right; font-style: italic; background-color: lightgray; }
  </style>
</head>
<body>
  <h1>The aside element</h1>
  <p>今年夏天，我和我的家人参观了 未来世界中心。 天气很好，Epcot 很棒！ 我和家人一起度过了一个美好的夏天！</p>
  <aside>
    <p>HTML的全称为超文本标记语言，是一种标记语言。它包括一系列标签．通过这些标签可以将网络上的文档格式统一，使分散的 Internet 资源连接为一个逻辑整体。</p>
  </aside>
  <p>今年夏天，我和我的家人参观了 未来世界中心。 天气很好，Epcot 很棒！ 我和家人一起度过了一个美好的夏天！</p>
  <p>今年夏天，我和我的家人参观了 未来世界中心。 天气很好，Epcot 很棒！ 我和家人一起度过了一个美好的夏天！</p>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<aside>` 元素：

```css
aside {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg