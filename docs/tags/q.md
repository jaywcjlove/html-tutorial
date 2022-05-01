HTML \<q> 标签
===

## 示例

标记一个简短的报价：

```html idoc:preview
<p>世界自然基金会的目标是：
<q>建设一个人与自然和谐相处的未来。</q>
  我们希望他们成功。</p>
```

## 定义和用法

`<q>` 标签定义了一个短引号。

浏览器通常会在引号周围插入引号。

**提示：** 使用 [\<blockquote>](./blockquote.md) 进行长引用。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<q>    | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [cite](./q_cite.md) | *URL* | 指定报价的来源 URL |

## 全局属性

`<q>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<q>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例

使用 CSS 设置 \<q> 元素的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    q {
      color: gray;
      font-style: italic;
    }
  </style>
</head>
<body>
  <p>世界自然基金会的目标是：
  <q>建设一个人与自然和谐相处的未来。</q>
   我们希望他们成功。</p>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<q>` 元素：

```css
q {
  display: inline;
}
q:before {
  content: open-quote;
}
q:after {
  content: close-quote;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg