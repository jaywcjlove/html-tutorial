HTML 属性 Attributes
===

HTML 属性提供有关 HTML 元素的附加信息。

## HTML 属性

* 所有 HTML 元素都可以有**属性**
* 属性提供有关元素的**附加信息**
* 属性总是在**开始标签**中指定
* 属性通常以名称/值对的形式出现，例如：**name="value"**

## href 属性

`<a>` 标签定义了一个超链接。 `href` 属性指定链接到的页面的 URL：

```html idoc:preview:iframe
<a href="https://github.com/jaywcjlove/html-tutorial">访问教程源码</a>
```

您将在我们的 [HTML 链接章节](./links.md) 中了解有关链接的更多信息。

## src 属性

`<img>` 标签用于在 HTML 页面中嵌入图像。 `src` 属性指定要显示的图像的路径：

```html idoc:preview:iframe
<img src="../assets/chrome.svg" >
```

有两种方法可以在 `src` 属性中指定 URL：

**1). 绝对 URL** - 指向托管在另一个网站上的外部图像的链接。 示例：`src="https://www.example.com/assets/chrome.svg"`。

**注意：** 外部图像可能受版权保护。 如果您没有获得使用许可，您可能违反了版权法。 此外，您无法控制外部图像； 它可以突然被删除或更改。

**2). 相对 URL** - 链接到网站内托管的图像。 此处，URL 不包含域名。 如果 URL 开头没有斜杠，则它将相对于当前页面。 示例：`src="chrome.svg"`。 如果 URL 以斜杠开头，它将与域相关。 示例：`src="/assets/chrome.svg"`。

**提示：** 几乎总是最好使用相对 URL。 如果您更改域，它们不会中断。

## 宽度 width 和高度 height 属性

`<img>` 标签还应该包含 `width` 和 `height` 属性，它们指定图像的宽度和高度（以像素为单位）：

```html idoc:preview:iframe
<img
  src="../assets/chrome.svg"
  width="120"
  height="120"
  alt="谷歌浏览器">
```

## 替代文本 alt 属性

如果由于某种原因无法显示图像，则 `<img>` 标签所需的 `alt` 属性指定图像的替代文本。 这可能是由于连接速度较慢，或者 `src` 属性中的错误，或者如果用户使用屏幕阅读器。

```html idoc:preview:iframe
<img src="../assets/chrome.svg" alt="谷歌浏览器">
```

看看如果我们尝试显示一个不存在的图像会发生什么：

```html idoc:preview:iframe
<img src="../assets/chrome111.svg" alt="谷歌浏览器">
```

您将在我们的 [HTML 图片章节](./images.md) 中了解有关图片的更多信息。


## 样式 style 属性

`style` 属性用于为元素添加样式，例如颜色、字体、大小等。

```html idoc:preview:iframe
<p style="color:red;">这是一个红色的段落。</p>
```

您将在我们的 [HTML 样式章节](./styles.md) 中了解有关样式的更多信息。

## 语言 lang 属性

您应该始终在 `<html>` 标签中包含 `lang` 属性，以声明网页的语言。 这是为了帮助搜索引擎和浏览器。

以下示例将英语指定为语言：

```html
<!DOCTYPE html>
<html lang="en">
<body>
  ...
</body>
</html>
```

国家代码也可以添加到 `lang` 属性中的语言代码中。 因此，前两个字符定义 HTML 页面的语言，后两个字符定义国家。

以下示例将 en 英语指定为语言，将 `CN` 指定为国家：

```html
<!DOCTYPE html>
<html lang="en-CN">
<body>
  ...
</body>
</html>
```

您可以在我们的 [HTML 语言代码参考](../reference/language_codes.md) 中查看所有语言代码。

## 标题 title 属性

`title` 属性定义了一些关于元素的额外信息。

当您将鼠标悬停在元素上时，title 属性的值将显示为工具提示：

```html
<p title="我是工具提示">这是一个段落。</p>
```

```html idoc:preview:iframe
<h2 title="我是标题">标题属性</h2>

<p title="我是工具提示">
  将鼠标悬停在此段落上，将标题属性显示为工具提示。
</p>
```

## 我们建议：始终使用小写属性

HTML 标准不需要小写的属性名称。

标题属性（和所有其他属性）可以用大写或小写写成，如 **title** 或 **TITLE**。

然而，W3C **建议** HTML 中的小写属性，并且**要求**小写属性用于更严格的文档类型，例如 XHTML。

在 W3Schools，我们总是使用小写的属性名称。

## 我们建议：始终引用属性值

HTML 标准不需要在属性值周围加上引号。

但是，W3C **建议** HTML 中使用引号，而 **要求** XHTML 等更严格的文档类型使用引号。

### 👍 正确:

```html
<a href="https://github.com/jaywcjlove/html-tutorial">访问我们的 HTML 教程</a>
```

### 👎 错误:

```html
<a href=https://github.com/jaywcjlove/html-tutorial>访问我们的 HTML 教程</a>
```
<!--rehype:style=background-color: #ff00004d;-->

有时你必须使用引号。 此示例将无法正确显示 title 属性，因为它包含空格：

### 实例

```html
<p title=关于 教程>
```

```html idoc:preview:iframe
<p title=关于 教程>
您不能在属性值周围省略引号
如果值包含空格。
</p>

<p><b>
如果将鼠标移到上面的段落上，
您的浏览器只会显示标题中的第一个"关于"。
</b></p>
```

在我们教程中，我们总是在属性值周围使用引号。

## 单引号还是双引号？

属性值周围的 `双引号` 在 HTML 中最常见，但也可以使用 `单引号`。

在某些情况下，当属性值本身包含`双引号` 时，需要使用 `单引号`：

```html
<p title='这是 "标题" 内容'>
```

或相反亦然：

```html
<p title="这是 '标题' 内容">
```

## 章节总结

* 所有 HTML 元素都可以有**属性**
* `<a>` 的 `href` 属性指定链接指向的页面的 URL
* `<img>`的`src`属性指定要显示的图片的路径
* `<img>` 的 `width` 和 `height` 属性提供图片的尺寸信息
* `<img>` 的 `alt` 属性为图像提供替代文本
* `style` 属性用于为元素添加样式，例如颜色、字体、大小等
* `<html>`标签的`lang`属性声明了网页的语言
* `title` 属性定义了一些关于元素的额外信息

## HTML 属性参考

每个 HTML 元素的所有属性的完整列表在我们的：[HTML 属性参考](../reference/attributes.md) 中列出。
