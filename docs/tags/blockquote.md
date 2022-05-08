HTML \<blockquote> 标签
===

## 示例

从另一个来源引用的部分：

```html idoc:preview
<blockquote cite="http://www.worldwildlife.org/who/index.html">
50 年来，WWF 一直在保护自然的未来。 作为世界领先的保护组织，WWF 在 100 个国家开展工作，并得到美国 120 万会员和全球近 500 万会员的支持。
</blockquote>
```

## 定义和用法

`<blockquote>` 标签指定从另一个来源引用的部分。

浏览器通常会缩进 `<blockquote>` 元素（查看下面的示例以了解如何删除缩进）。

## 提示和注意事项

**提示：** 使用 `<q>` 进行内联（短）引用。

## 浏览器支持

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------------- | --- | --- | --- | --- | --- |
| \<blockquote> | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [cite](./blockquote_cite.md) | *URL* | 规定引用的来源。 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<blockquote>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<blockquote>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 从 `blockquote` 元素中删除缩进：

```html idoc:preview:iframe
<html>
<head>
  <style>
    blockquote { margin-left:0; }
  </style>
</head>
<body>
  <p>以下是来自 WWF 网站的引述：</p>
  <blockquote cite="http://www.worldwildlife.org/who/index.html">
  50 年来，WWF 一直在保护自然的未来。 作为世界领先的保护组织，WWF 在 100 个国家开展工作，并得到美国 120 万会员和全球近 500 万会员的支持。
  </blockquote>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<blockquote>` 元素：

```css
blockquote {
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