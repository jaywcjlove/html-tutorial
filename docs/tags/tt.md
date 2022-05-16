HTML \<tt> 标签
===

[![](https://shields.io/badge/HTML5-已弃用/过时-yellow?logo=HTML5)](https://caniuse.com/?search=<tt>)

## HTML5 不支持

`<tt>` 标签在 HTML 4 中呈现类似打字机或者等宽的文本效果。

## 改用什么？

考虑 [\<kbd>](./kbd.md) 元素（用于键盘输入）、[\<var>](./var.md) 元素（用于变量）、[\<code>](./code.md) 元素（用于计算机代码）、[\<samp>](./samp.md) 元素（用于计算机输出），或者改用 CSS。

### Example

为 \<p> 元素定义电传打字机/等宽字体（使用 CSS）：

```html idoc:preview:iframe
<p style="font-family:'Lucida Console', monospace">This text is monospace text.</p>
```