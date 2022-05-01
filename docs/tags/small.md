HTML \<small> Tag
===

## 示例

定义一个较小的文本：

```html idoc:preview:iframe
<p>这是一些普通的文字。</p>
<p><small>这是一些较小的文本。</small></p>
```

## 定义和用法

`<small>` 标签定义较小的文本（如版权和其他旁注）。

**提示：** 此标签并未被弃用，但可以通过 CSS 实现更丰富（或相同）的效果。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<small> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<small>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<small>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 定义较小的文本：

```html idoc:preview:iframe
<html>
<head>
  <style>
    span.small {
      font-size: smaller;
    }
  </style>
</head>
<body>
  <p>这是一些普通的文字。</p>
  <p><small>这是一些较小的文本。</small></p>
</body>
</html>
```

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<script>` 元素：

```css
small {
  font-size: smaller;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg