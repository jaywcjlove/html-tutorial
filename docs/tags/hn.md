HTML \<h1> to \<h6> Tags
===

## 示例

六个不同的 HTML 标题：

```html idoc:preview
<h1>这是标题 1</h1>
<h2>这是标题 2</h2>
<h3>这是标题 3</h3>
<h4>这是标题 4</h4>
<h5>这是标题 5</h5>
<h6>这是标题 6</h6>
```
<!--rehype:style=min-height: 350px;-->

## 定义和用法

`<h1>` 到 `<h6>` 标签用于定义 HTML 标题。

`<h1>` 定义了最重要的标题。 `<h6>` 定义了最不重要的标题。

**注意：** 每页只使用一个 `<h1>` - 这应该代表整个页面的主要标题/主题。 此外，不要跳过标题级别 - 从 `<h1>` 开始，然后使用 `<h2>`，依此类推。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<h1> - \<h6> | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<h1>` ~ `<h6>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<h1>` ~ `<h6>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

设置标题的背景颜色和文本颜色（使用 CSS）：

```html idoc:preview
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<h2 style="color:Tomato;">Hello World</h2>
```
<!--rehype:style=min-height: 190px;-->

设置标题的对齐方式（使用 CSS）：

```html idoc:preview
<h1 style="text-align:center">这是标题 1</h1>
<h2 style="text-align:left">这是标题 2</h2>
<h3 style="text-align:right">这是标题 3</h3>
<h4 style="text-align:justify">这是标题 4</h4>
```
<!--rehype:style=min-height: 290px;-->

## 相关页面

HTML tutorial: [HTML Headings](../tutorial/headings.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<h1>` 元素：

```css
h1 {
  display: block;
  font-size: 2em;
  margin-top: 0.67em;
  margin-bottom: 0.67em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

大多数浏览器将显示具有以下默认值的 `<h2>` 元素：

```css
h2 {
  display: block;
  font-size: 1.5em;
  margin-top: 0.83em;
  margin-bottom: 0.83em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

大多数浏览器将显示具有以下默认值的 `<h3>` 元素：

```css
h3 {
  display: block;
  font-size: 1.17em;
  margin-top: 1em;
  margin-bottom: 1em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

大多数浏览器将显示具有以下默认值的 `<h4>` 元素：

```css
h4 {
  display: block;
  font-size: 1em;
  margin-top: 1.33em;
  margin-bottom: 1.33em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

大多数浏览器将显示具有以下默认值的 `<h5>` 元素：

```css
h5 {
  display: block;
  font-size: .83em;
  margin-top: 1.67em;
  margin-bottom: 1.67em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

大多数浏览器将显示具有以下默认值的 `<h6>` 元素：

```css
h6 {
  display: block;
  font-size: .67em;
  margin-top: 2.33em;
  margin-bottom: 2.33em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg