HTML \<details> Tag
===

## 示例

指定用户可以按需打开和关闭的详细信息：

```html idoc:preview:iframe
<details>
  <summary>HyperText Markup Language</summary>
  <p>超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。</p>
</details>
```

## 定义和用法

`<details>` 标记指定用户可以按需打开和关闭的其他详细信息。

`<details>` 标签通常用于创建用户可以打开和关闭的交互式小部件。 默认情况下，小部件是关闭的。 打开时，它会展开并显示其中的内容。

任何类型的内容都可以放在`<details>` 标签内。

**提示：** [\<summary>](./summary.md) 标签与 `<details>` 结合使用，以指定详细信息的可见标题。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<details> | 12.0 | 79.0 | 49.0 | 6.0 | 15.0 |

## 全局属性

`<details>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<details>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<details> 和 [\<summary>](./summary.md) 的样式：

```html idoc:preview:iframe
<html>
<style>
  details > summary {
    padding: 4px;
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
<body>
  <details>
    <summary>HyperText Markup Language</summary>
    <p>超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。</p>
  </details>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<details>` 元素：

```css
details {
  display: block;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg