HTML \<main> Tag
===

## 示例

指定文档的主要内容：

```html idoc:preview:iframe
<main>
  <h1>最受欢迎的浏览器</h1>
  <p>Chrome、Firefox 和 Edge 是当今最常用的浏览器。</p>
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
    <p>Microsoft Edge 是 Microsoft 开发的 Web 浏览器，于 2015 年发布。Microsoft Edge 取代了 Internet Explorer。</p>
  </article>
</main>
```

## 定义和用法

`<main>` 标签指定文档的主要内容。

`<main>` 元素内的内容对于文档应该是唯一的。 它不应包含在文档中重复的任何内容，例如侧边栏、导航链接、版权信息、站点徽标和搜索表单。

**注意：** 文档中的 `<main>` 元素不得超过一个。 `<main>` 元素不能是 [\<article>](./article.md)、[\<aside>](./aside.md)、[\<footer>](./footer.md)、[\<header>](./header.md) 或 [\<nav>](./nav.md) 元素的后代。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<main> | 26.0 | 12.0 | 21.0 | 7.0 | 16.0 |

## 全局属性

`<main>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<main>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例

使用 CSS 设置 \<main> 元素的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    main {
      margin: 0;
      padding: 5px;
      background-color: lightgray;
    }
    main > h1, p, .browser {
      margin: 10px;
      padding: 5px;
    }
    .browser {
      background: white;
    }
    .browser > h2, p {
      margin: 4px;
      font-size: 90%;
    }
  </style>
</head>
<body>
  <main>
    <h1>最受欢迎的浏览器</h1>
    <p>Chrome、Firefox 和 Edge 是当今最常用的浏览器。</p>
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
      <p>Microsoft Edge 是 Microsoft 开发的 Web 浏览器，于 2015 年发布。Microsoft Edge 取代了 Internet Explorer。</p>
    </article>
  </main>
</body>
</html>
```
<!--rehype:style=height: 480px;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg