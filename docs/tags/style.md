HTML \<style> 标签
===

## 示例

使用 \<style> 元素将简单的样式表应用于 HTML 文档：

```html idoc:preview:iframe
<html>
<head>
  <style>
    h1 {color:red;}
    p {color:blue;}
  </style>
</head>
<body>
  <h1>A heading</h1>
  <p>A paragraph.</p>
</body>
</html>
```
<!--rehype:style=height: 130px;-->

## 定义和用法

`<style>` 标签用于定义文档的样式信息 (CSS)。

在 `<style>` 元素中，您可以指定 HTML 元素应如何在浏览器中呈现。

## 提示和注意事项

**注意：** 浏览器在读取样式表时，会根据样式表中的信息对 HTML 文档进行格式化。 如果在不同的样式表中为相同的选择器（元素）定义了一些属性，则将使用上次读取的样式表中的值（参见下面的示例）！

**提示：** 要链接到外部样式表，请使用 [\<link>](./link.md) 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<style> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [media](./style_media.md) | *media\_query* | 指定媒体资源优化的媒体/设备 |
| [type](./style_type.md)   | text/css | 指定 \<style> 标签的媒体类型 |

## 全局属性

`<style>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<style>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

相同元素的多种样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    h1 {color:red;}
    p {color:blue;}
  </style>
  <style>
    h1 {color:green;}
    p {color:pink;}
  </style>
</head>
<body>
  <h1>This is a heading</h1>
  <p>This is a paragraph.</p>
</body>
</html>
```
<!--rehype:style=height: 130px;-->

## 相关页面

HTML 教程: [HTML CSS](../tutorial/css.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<style>` 元素：

```css
style {
  display: none;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg