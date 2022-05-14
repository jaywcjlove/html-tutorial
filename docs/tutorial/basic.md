HTML 基础示例
===

在本章中，我们将展示一些基本的 HTML 示例。

如果我们使用您尚未了解的标签，请不要担心。

## HTML 文档

所有 HTML 文档都必须以文档类型声明开头：[`<!DOCTYPE html>`](../tags/doctype.md)。

HTML 文档本身以 `<html>` 开头并以 `</html>` 结尾。

HTML 文档的可见部分位于 `<body>` 和 `</body>` 之间。

### 示例

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body>
  <h1>我的第一个标题</h1>
  <p>我的第一段落。</p>
</body>
</html>
```

## \<!DOCTYPE> 声明

`<!DOCTYPE>` 声明表示文档类型，并帮助浏览器正确显示网页。

它只能出现一次，在页面顶部（在任何 HTML 标记之前）。

`<!DOCTYPE>` 声明不区分大小写。

HTML5 的 `<!DOCTYPE>` 声明是：

```html
<!DOCTYPE html>
```

## HTML 标题

HTML 标题是用 `<h1>` 到 `<h6>` 标签定义的。

`<h1>` 定义了最重要的标题。 `<h6>` 定义了最不重要的标题：

```html
<h1>这是标题 1</h1>
<h2>这是标题 2</h2>
<h3>这是标题 3</h3>
```

```html idoc:preview:iframe
<h1>这是标题 1</h1>

<h2>这是标题 2</h2>

<h3>这是标题 3</h3>
```

## HTML 段落

HTML 段落使用 `<p>` 标签定义：

```html
<p>这是一个段落。</p>
<p>这是另一段。</p>
```

```html idoc:preview:iframe
<p>这是一个段落。</p>
<p>这是另一段。</p>
```

## HTML 链接

HTML 链接使用 `<a>` 标签定义：

```html
<a href="https://github.com/jaywcjlove/html-tutorial">这是一个链接</a>
```

```html idoc:preview
<a href="https://github.com/jaywcjlove/html-tutorial">这是一个链接</a>
```

链接的目的地在 `href` 属性中指定。

属性用于提供有关 HTML 元素的附加信息。

您将在后面的章节中了解有关属性的更多信息。

## HTML 图像

HTML 图像使用 `<img>` 标签定义。

源文件 (`src`)、替代文本 (`alt`)、`width` 和 `height` 作为属性提供：

```html
<img src="../assets/chrome.svg" alt="Chrome 浏览器" width="104" height="104">
```

```html idoc:preview
<img
  src="../assets/chrome.svg"
  alt="Chrome 浏览器"
  width="104"
  height="104"
>
```

## 如何查看 HTML 源代码？

您是否曾经看过一个网页并想知道“嘿！他们是怎么做到的？”

### 查看 HTML 源代码：

在 HTML 页面中单击鼠标右键，然后选择 `查看页面源代码`（在 Chrome 中）或 `查看源代码`（在 Edge 中），或在其他浏览器中类似。 这将打开一个包含页面 HTML 源代码的窗口。

### 检查一个 HTML 元素：

右键单击一个元素（或空白区域），然后选择 `检查` 或 `检查元素` 以查看由哪些元素组成（您将看到 HTML 和 CSS）。 您还可以在打开的 `元素` 或 `样式` 面板中即时编辑 HTML 或 CSS。