HTML `title` 属性
===

指定有关元素的额外信息。

## 实例

在 HTML 文档中使用 `title` 属性：

```html idoc:preview
<abbr title="People's Republic of China">PRC</abbr> was founded in 1949.
<p title="Free Web tutorials">HTML Tutorial</p>
```

## 定义和使用

`title` 属性指定有关元素的额外信息。

当鼠标移到元素上时，该信息通常显示为工具提示文本。

`title` 属性可用于任何 HTML 元素（它将在任何 HTML 元素上验证。但是，它不一定有用）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;title&gt;__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element title="text">
```

## 属性值

值 Value | 描述 Description
---- | ----
text | 元素的工具提示文本

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg