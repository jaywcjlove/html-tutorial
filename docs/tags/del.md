HTML \<del> Tag
===

## 示例

具有已删除部分和新插入部分的文本：

```html idoc:preview:iframe
<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>
```

## 定义和用法

`<del>` 标签定义已从文档中删除的文本。 浏览器通常会删除已删除的文本。

## 提示和注意事项

**提示：** 还要查看 [\<ins>](./ins.md) 标记以标记插入的文本。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<del>  | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| [cite](./del_cite.md)         | *URL*                    | 指定一个文档的 URL，该文档解释了文本被删除/更改的原因 |
| [datetime](./del_datetime.md) | *YYYY-MM-DDThh:mm:ssTZD* | 指定删除/更改文本的日期和时间 |

## 全局属性

`<del>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<del>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 来设置 \<del> 和 \<ins> 的样式：

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

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<del>` 元素：

```css
del {
  text-decoration: line-through;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg