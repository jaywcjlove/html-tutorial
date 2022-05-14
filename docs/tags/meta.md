HTML \<meta> 标签
===

## 示例

描述 HTML 文档中的元数据：

```html
<head>
  <meta charset="UTF-8">
  <meta name="description" content="Free Web tutorials">
  <meta name="keywords" content="HTML, CSS, JavaScript">
  <meta name="author" content="John Doe">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
```

## 定义和用法

`<meta>` 标签定义关于 HTML 文档的元数据。 元数据是关于数据的数据（信息）。

`<meta>` 标签始终位于 [\<head>](./head.md) 元素内，通常用于指定字符集、页面描述、关键字、文档作者和视口设置。

元数据不会显示在页面上，但机器可解析。

元数据由浏览器（如何显示内容或重新加载页面）、搜索引擎（关键字）和其他 Web 服务使用。

有一种方法可以让网页设计师通过 `<meta>` 标签控制视口（网页的用户可见区域）（参见下面的“设置 Viewport”示例）。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<meta> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [charset](./meta_charset.md)       | *character\_set* | 指定 HTML 文档的字符编码 |
| [content](./meta_content.md)       | *text* | 指定与 http-equiv 或 name 属性关联的值 |
| [http-equiv](./meta_http_equiv.md) | content-security-policy<br>content-type<br>default-style<br>refresh       | 为内容属性的信息/值提供 HTTP 标头 |
| [name](./meta_name.md)             | application-name<br>author<br>description<br>generator<br>keywords<br>viewport | 指定元数据的名称 |

## 全局属性

`<meta>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 更多示例

**为搜索引擎定义关键字：**

```html
<meta name="keywords" content="HTML, CSS, JavaScript">
```

**定义您的网页描述：**

```html
<meta name="description" content="Free Web tutorials for HTML and CSS">
```

**定义页面的作者：**

```html
<meta name="author" content="John Doe">
```

**每 30 秒刷新一次文档：**

```html
<meta http-equiv="refresh" content="30">
```

**设置视口以使您的网站在所有设备上看起来都不错：**

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## 设置 Viewport

Viewport 是网页的用户可见区域。 它因设备而异 - 在手机上会比在电脑屏幕上小。

您应该在所有网页中包含以下 `<meta>` 元素：

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

这为浏览器提供了有关如何控制页面尺寸和缩放的说明。

- `width=device-width` 部分设置页面的宽度以跟随设备的屏幕宽度（这将因设备而异）。
- `initial-scale=1.0` 部分设置浏览器首次加载页面时的初始缩放级别。

这是一个网页示例 *`没有`* viewport 元标记，以及同一个网页 *`带有`* viewport 元标记：

**提示：** 如果您是用手机或平板电脑浏览此页面，您可以点击下面的两个链接查看不同之处。

没有 viewport 元标签 | 使用 viewport 元标签
---- | ----
![](../assets/responsive_viewport1.png) | ![](../assets/responsive_viewport2.png)

## 相关页面

HTML 教程: [HTML Head](../tutorial/head.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg