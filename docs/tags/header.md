HTML \<header> 标签
===

## 示例

\<article> 的标题：

```html idoc:preview
<article>
  <header>
    <h1>这里有个标题</h1>
    <p>Posted by Hello World</p>
    <p>这里有一些额外的信息</p>
  </header>
  <p>这里有一些额外的信息....</p>
</article>
```
<!--rehype:style=min-height: 210px;-->

## 定义和用法

`<header>` 元素表示介绍性内容或一组导航链接的容器。

`<header>` 元素通常包含：

* 一个或多个标题元素 ([\<h1>](./hn.md) ~ [\<h6>](./hn.md))
* 标志或图标
* 作者信息

**注意：** 您可以在一个 HTML 文档中包含多个 `<header>` 元素。 但是，`<header>` 不能放在 [\<footer>](./footer.md)、[\<address>](./address.md) 或另一个 `<header>` 元素中。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<header> | 5.0 | 9.0 | 4.0 | 5.0 | 11.1 |

## 全局属性

`<header>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<header>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

页眉：

```html idoc:preview
<header>
  <h1>主页标题在这里</h1>
  <p>Posted by Hello World</p>
</header>
```
<!--rehype:style=min-height: 160px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<header>` 元素：

```css
header {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg