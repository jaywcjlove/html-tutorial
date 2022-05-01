HTML \<pre> 标签
===

## 示例

预格式化文本：

```html idoc:preview
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>
```

## 定义和用法

`<pre>` 标签定义了预格式化的文本。

`<pre>` 元素中的文本以固定宽度字体显示，并且文本同时保留空格和换行符。 文本将完全按照 HTML 源代码中的内容显示。

还请看：

| 标签 Tag | 描述 Description |
| ---- | ---- |
| [\<code>](./code.md) | 定义一段计算机代码 |
| [\<samp>](./samp.md) | 定义计算机程序的样本输出 |
| [\<kbd>](./kbd.md)   | 定义键盘输入 |
| [\<var>](./var.md)   | 定义一个变量 |

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<pre>  | Yes | Yes | Yes | Yes | Yes |


## 全局属性

`<pre>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<pre>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

如何创建具有固定宽度的预格式化文本（使用 CSS）：

```html idoc:preview
<div style="width:200px; overflow:auto">
  <pre>This is a pre with a fixed width. It will use as much space as specified.</pre>
</div>
```

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<pre>` 元素：

```css
pre {
  display: block;
  font-family: monospace;
  white-space: pre;
  margin: 1em 0;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg