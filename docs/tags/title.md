HTML \<title> Tag
===

## 示例

为您的 HTML 文档定义一个标题：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <title>HTML Elements Reference</title>
</head>
<body>
  <h1>This is a heading</h1>
  <p>This is a paragraph.</p>
</body>
</html>
```

## 定义和用法

`<title>` 标签定义了文档的标题。标题必须是纯文本的，并且显示在浏览器的标题栏或页面的选项卡中。

HTML 文档中需要 `<title>` 标签！

页面标题的内容对于搜索引擎优化 (SEO) 非常重要！搜索引擎算法使用页面标题来决定在搜索结果中列出页面时的顺序。

`<title>` 元素：

* 在浏览器工具栏中定义一个标题
* 为页面添加到收藏夹时提供标题
* 在搜索引擎结果中显示页面的标题

以下是创建好标题的一些技巧：

* 选择更长的描述性标题（避免使用一个或两个单词的标题）
* 搜索引擎会显示大约 50-60 个字符的标题，所以尽量不要让标题长于那个
* 不要只使用单词列表作为标题（这可能会降低页面在搜索结果中的位置）

所以，尽量使标题尽可能准确和有意义！

**注意：** HTML 文档中不能有多个 `<title>` 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<title> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<title>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## Related Pages

HTML 教程: [HTML Head](../tutorial/head.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<title>` 元素：

```css
title {
  display: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg