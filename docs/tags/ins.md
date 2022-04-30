HTML \<ins> Tag
===

## 示例

具有已删除部分和新插入部分的文本：

```html idoc:preview
<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>
```

## 定义和用法

`<ins>` 标签定义了已插入文档的文本。 浏览器通常会在插入的文本下划线。

**提示：** 另请查看 [\<del>](./del.md) 标记以标记已删除的文本。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<ins>  | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [cite](att_ins_cite.asp)         | *URL*                    | 指定文档的 URL，该文档解释了插入/更改文本的原因 |
| [datetime](att_ins_datetime.asp) | *YYYY-MM-DDThh:mm:ssTZD* | 指定插入/更改文本的日期和时间 |

## 全局属性

`<ins>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<ins>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<del> 和 \<ins> 的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    del {background-color: tomato;}
    ins {background-color: yellow;}
  </style>
</head>
<body>
  <p>My favorite color is <del>blue</del> <ins>red</ins>!</p>
</body>
</html>
```
<!--rehype:style=height: 120px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<ins>` 元素：

```css
ins {
  text-decoration: underline;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg