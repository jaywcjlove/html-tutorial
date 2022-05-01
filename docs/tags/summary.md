HTML \<summary> Tag
===

## 示例

使用 \<summary> 元素：

```html idoc:preview:iframe
<details>
  <summary>
    HyperText Markup Language
  </summary>
  <p>HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）</p>
</details>
```

## 定义和用法

`<summary>` 标记定义了 [\<details>](./details.md) 元素的可见标题。 可以单击标题以查看/隐藏详细信息。

**注意：** `<summary>` 元素应该是 [\<details>](./details.md) 元素的第一个子元素。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<summary> | 12.0 | 79.0 | 49.0 | 6.0 | 15.0 |

## 全局属性

`<summary>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<summary>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 [\<details>](./details.md) 和 \<summary> 的样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    details > summary {
      padding: 4px;
      width: 200px;
      background-color: #eeeeee;
      border: none;
      box-shadow: 1px 1px 2px #bbbbbb;
      cursor: pointer;
    }
    details > p {
      background-color: #eeeeee;
      padding: 4px;
      margin: 0;
      box-shadow: 1px 1px 2px #bbbbbb;
    }
  </style>
</head>
<body>
  <details>
    <summary>HyperText Markup Language</summary>
    <p>HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）</p>
  </details>
</body>
</html>
```
<!--rehype:style=height: 230px;-->

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<summary>` 元素：

```css
summary {
  display: block;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg