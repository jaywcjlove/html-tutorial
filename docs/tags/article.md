HTML \<article> 标签
===

## 示例

三篇内容独立、自成一体的文章：

```html idoc:preview:iframe
<article>
<h2>Google Chrome</h2>
<p>Google Chrome 是谷歌开发的网络浏览器，于 2008 年发布。Chrome 是当今世界上最受欢迎的网络浏览器！</p>
</article>

<article>
<h2>Mozilla Firefox</h2>
<p>Mozilla Firefox 是 Mozilla 开发的开源网络浏览器。 自 2018 年 1 月以来，Firefox 一直是第二受欢迎的网络浏览器。</p>
</article>

<article>
<h2>Microsoft Edge</h2>
<p>Microsoft Edge 是微软开发的一款网络浏览器，于 2015 年发布。Microsoft Edge 取代了 Internet Explorer。</p>
</article>
```

## 定义和用法

`<article>` 标签指定独立的、自包含的内容。

一篇文章本身应该有意义，并且应该可以独立于网站的其余部分进行分发。

`<article>` 元素的潜在来源：

* 论坛帖子
* 博客文章
* 新闻故事

**注意：** `<article>` 元素在浏览器中不会呈现为任何特殊内容。 但是，您可以使用 CSS 来设置 `<article> `元素的样式（参见下面的示例）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __\<article>__ | 6.0 | 9.0 | 4.0 | 5.0 | 11.1 |

## 全局属性

`<article>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<article>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例

使用 CSS 设置 \<article> 元素的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    .all-browsers { margin: 0; padding: 5px; background-color: lightgray; }
    .all-browsers > h1, .browser { margin: 10px; padding: 5px; }
    .browser { background: white; }
    .browser > h2, p { margin: 4px; font-size: 90%; }
  </style>
</head>
<body>
<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome 是谷歌开发的网络浏览器，于 2008 年发布。Chrome 是当今世界上最受欢迎的网络浏览器！</p>
  </article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox 是 Mozilla 开发的开源网络浏览器。 自 2018 年 1 月以来，Firefox 一直是第二受欢迎的网络浏览器。</p>
  </article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge 是微软开发的一款网络浏览器，于 2015 年发布。Microsoft Edge 取代了 Internet Explorer。</p>
  </article>
</article>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<article>` 元素：

```css
article {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg