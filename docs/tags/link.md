HTML \<link> Tag
===

## 示例

链接到外部样式表：

```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

## 定义和用法

`<link>` 标签定义了当前文档和外部资源之间的关系。

`<link>` 标签最常用于链接到外部样式表或将 [favicon](../tutorial/favicon.md) 添加到您的网站。

`<link>` 元素是一个空元素，它只包含属性。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<link> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| crossorigin                                     | anonymous use-credentials | 指定元素如何处理跨域请求 |
| [href](att_link_href.asp)                       | *URL* | 指定链接文档的位置 |
| [hreflang](att_link_hreflang.asp)               | *language\_code* | 指定链接文档中文本的语言 |
| [media](att_link_media.asp)                     | *media\_query* | 指定链接文档将在什么设备上显示 |
| [referrerpolicy](att_iframe_referrerpolicy.asp) | no-referrer<br>no-referrer-when-downgrade<br>origin<br>origin-when-cross-origin<br>unsafe-url | 指定在获取资源时使用哪个引用者 |
| [rel](att_link_rel.asp)                         | alternate<br>author<br>dns-prefetch<br>help<br>icon<br>license<br>next<br>pingback<br>preconnect<br>prefetch<br>preload<br>prerender<br>prev<br>search<br>stylesheet | 必需的，指定当前文档和链接文档之间的关系|
| [sizes](att_link_sizes.asp)                     | *Height* x *Width* <br>any | 指定链接资源的大小。 仅适用于 rel="icon" |
| title                                           || 定义首选或备用样式表 |
| [type](att_link_type.asp)                       | *media\_type*| 指定链接文档的媒体类型 |

## 全局属性

`<link>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<link>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Styles](../tutorial/css.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<link>` 元素：

```css
link {
  display: none;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg