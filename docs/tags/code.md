HTML \<code> Tag
===

## 示例

将一些文本定义为文档中的计算机代码：

```html idoc:preview
<p>The HTML <code>button</code> tag defines a clickable button.</p>
<p>The CSS <code>background-color</code> property defines the background color of an element.</p>
```

## 定义和用法

`<code>` 标签用于定义一段计算机代码。 里面的内容以浏览器默认的等宽字体显示。

**提示：** 此标签未被弃用。 但是，使用 CSS 可以实现更丰富的效果（参见下面的示例）。

还请看：

| 标签 Tag | 描述 Description |
| ------ | ----- |
| [\<samp>](./samp.md) | 定义计算机程序的样本输出 |
| [\<kbd>](./kbd.md)   | 定义键盘输入 |
| [\<var>](./var.md)   | 定义一个变量 |
| [\<pre>](./pre.md)   | 定义预格式化文本 |

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<code> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<code>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<code>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<code> 元素的样式：

```html idoc:preview
<html>
<head>
  <style>
    code {
      font-family: Consolas,"courier new";
      color: crimson;
      background-color: #f1f1f1;
      padding: 2px;
      font-size: 105%;
    }
  </style>
</head>
<body>
  <p>The HTML <code>button</code> tag defines a clickable button.</p>
  <p>The CSS <code>background-color</code> property defines the background color of an element.</p>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<code>` 元素：

```css
code {
  font-family: monospace;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg