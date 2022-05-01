HTML \<s> Tag
===

## 示例

标记不再正确的文本：

```html idoc:preview
<p><s>Only 50 tickets left!</s></p>
<p>SOLD OUT!</p>
```

## Definition and Usage

`<s>` 标签指定不再正确、准确或相关的文本。 文本将通过一条线显示。

`<s>` 标签不应用于定义文档中已删除的文本，请使用 [\<del>](./del.md) 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<s>    | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<s>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<s>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Text Formatting](../tutorial/formatting.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<s>` 元素：

```css
s {
  text-decoration: line-through;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg