HTML \<hr> 标签
===

## 示例

使用 \<hr> 标签来定义内容的主题变化：

```html idoc:preview
<h1>网络的主要语言</h1>
<p>HTML 是用于创建网页的标准标记语言。 HTML 描述网页的结构，由一系列元素组成。 HTML 元素告诉浏览器如何显示内容。</p>
<hr>
<p>CSS 是一种描述 HTML 元素如何在屏幕、纸张或其他媒体中显示的语言。 CSS节省了很多工作，因为它可以一次控制多个网页的布局。</p>
<hr>
<p>JavaScript 是 HTML 和 Web 的编程语言。 JavaScript 可以更改 HTML 内容和属性值。 JavaScript 可以改变 CSS。 JavaScript 可以隐藏和显示 HTML 元素等等。</p>
```
<!--rehype:style=min-height: 390px;-->

## 定义和用法

`<hr>` 标签定义了 HTML 页面中的主题中断（例如主题转换）。

`<hr>` 元素通常显示为水平线，用于分隔 HTML 页面中的内容（或定义更改）。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<hr>   | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<hr>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<hr>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

对齐 \<hr> 元素（使用 CSS）：

```html idoc:preview
<hr style="width:50%;text-align:left;margin-left:0">
```

一个没有阴影的 \<hr> （使用 CSS）：

```html idoc:preview
<hr style="height:2px;border-width:0;color:gray;background-color:gray">
```
<!--rehype:style=min-height: 40px;-->

设置 \<hr> 元素的高度（使用 CSS）：

```html idoc:preview
<hr style="height:30px">
```
<!--rehype:style=min-height: 80px;-->

设置 \<hr> 元素的宽度（使用 CSS）：

```html idoc:preview
<hr style="width:50%">
```
<!--rehype:style=min-height: 80px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<hr>` 元素：

```css
hr {
  display: block;
  margin-top: 0.5em;
  margin-bottom: 0.5em;
  margin-left: auto;
  margin-right: auto;
  border-style: inset;
  border-width: 1px;
}
```