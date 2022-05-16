HTML \<samp> 标签
===

## 示例

将一些文本定义为文档中计算机程序的示例输出：

```html idoc:preview
<p>来自我电脑的消息：</p>

<p><samp>文件未找到<br>按 F1 继续</samp></p>
```

## 定义和用法

`<samp>` 标签用于定义计算机程序的样本输出。里面的内容以浏览器默认的等宽字体显示。

**提示：** 此标签未被弃用。但是，使用 CSS 可以实现更丰富的效果。

还请看：

| 标签 Tag | 描述 Description |
| ------ | ----- |
| [\<code>](./code.md) | 定义一段计算机代码 |
| [\<kbd>](./kbd.md)   | 定义键盘输入 |
| [\<var>](./var.md)   | 定义一个变量 |
| [\<pre>](./pre.md)   | 定义预格式化文本 |

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<samp> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<samp>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<samp>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<samp>` 元素：

```css
samp {
  font-family: monospace;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg