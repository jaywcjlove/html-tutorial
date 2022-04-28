HTML `style` 属性
===

是否要检查元素的拼写和语法。

## 实例

在 HTML 文档中使用 `style` 属性：

```html idoc:preview:iframe
<h1 style="color:blue;text-align:center;">This is a header</h1>
<p style="color:green;">This is a paragraph.</p>
```
<!--rehype:style=min-height: 130px;-->

## 定义和使用

`style` 属性指定元素的内联样式。

`style` 属性将覆盖全局设置的任何样式，例如 `<style>` 标签或外部样式表中指定的样式。

`style` 属性可以在任何 HTML 元素上使用（它将在任何 HTML 元素上验证。但是，它不一定有用）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;style&gt;__ | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<element style="style_definitions">
```

## 属性值

值 Value | 描述 Description
---- | ----
style_definitions | 一个或多个用分号分隔的 CSS 属性和值（例如 `style="color:blue;text-align:center"`）

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg