HTML \<u> Tag
===

## 示例

用 \<u> 标签标记拼写错误的单词：

```html idoc:preview:iframe
<p>This is some <u>mispeled</u> text.</p>
```

## 定义和用法

`<u>` 标记表示一些不清晰且样式与普通文本不同的文本，例如拼写错误的单词或中文文本中的专有名称。 里面的内容通常用下划线显示。 您可以使用 CSS 更改它（参见下面的示例）。

**提示：** 避免使用 `<u>` 元素，因为它可能与超链接混淆！

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<u>    | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<u>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<u>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 为拼写错误的文本设置样式：

```html idoc:preview:iframe
<html>
<head>
<style>
  .spelling-error {
    text-decoration-line: underline;
    text-decoration-style: wavy;
    text-decoration-color: red;
  }
</style>
</head>
<body>
  <p>This is some <u class="spelling-error">mispeled</u> text.</p>
</body>
</html>
```
<!--rehype:style=height: 80px;-->

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<u>` 元素：

```css
u {
  text-decoration: underline;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg