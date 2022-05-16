HTML \<var> 标签
===

## 示例

将一些文本定义为文档中的变量：

```html idoc:preview:iframe
<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>
```

## 定义和用法

`<var>` 标签用于在编程或数学表达式中定义变量。 里面的内容通常以*斜体*显示。

**提示：** 此标签未被弃用。 但是，使用 CSS 可以实现更丰富的效果。

还请看：

| 标签 Tag | 描述 Description |
| ---- | ---- |
| [\<code>](./code.md) | 定义一段计算机代码 |
| [\<samp>](./samp.md) | 定义计算机程序的样本输出 |
| [\<kbd>](./kbd.md)   | 定义键盘输入 |
| [\<pre>](./pre.md)   | 定义预格式化文本 |

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<var>  | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<var>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<var>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<var>` 元素：

```css
var {
  font-style: italic;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg