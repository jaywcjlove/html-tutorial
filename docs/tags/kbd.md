HTML \<kbd> 标签
===

## 示例

在文档中定义一些文本作为键盘输入：

```html idoc:preview:iframe
<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>

<p>Press <kbd>Cmd</kbd> + <kbd>C</kbd> to copy text (Mac OS).</p>
```

## 定义和用法

`<kbd>` 标签用于定义键盘输入。 里面的内容以浏览器默认的等宽字体显示。

**提示：** 此标签未被弃用。 但是，使用 CSS 可以实现更丰富的效果（参见下面的示例）。

还请看：

| 标签 Tag | 描述 Description |
| ---- | ---- |
| [\<code>](./code.md) | 定义一段计算机代码 |
| [\<samp>](./samp.md) | 定义计算机程序的样本输出 |
| [\<var>](./var.md)   | 定义一个变量 |
| [\<pre>](./pre.md)   | 定义预格式化文本 |

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<kbd>  | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<kbd>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<kbd>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<kbd> 元素的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    kbd {
      border-radius: 2px;
      padding: 2px;
      border: 1px solid black;
    }
  </style>
</head>
<body>
  <p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>
  <p>Press <kbd>Cmd</kbd> + <kbd>C</kbd> to copy text (Mac OS).</p>
</body>
</html>
```
<!--rehype:style=height: 130px;-->

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<kbd>` 元素：

```css
kbd {
  font-family: monospace;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg