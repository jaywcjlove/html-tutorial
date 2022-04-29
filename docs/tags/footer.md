HTML \<footer> 标签
===

## 示例

文档中的页脚部分：

```html idoc:preview
<footer>
  <p>Author: Hello World</p>
  <p><a href="mailto:hello@example.com">hello@example.com</a></p>
</footer>
```

## 定义和用法

`<footer>` 标签定义文档或部分的页脚。

`<footer>` 元素通常包含：

* 作者信息
* 版权信息
* 联系信息
* 网站地图
* 返回顶部链接
* 相关文件

您可以在一个文档中包含多个 `<footer>` 元素。

## 提示和注意事项

**提示：** `<footer>` 元素内的联系信息应放在 [\<address>](./address.md) 标记内。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<footer> | 5.0 | 9.0 | 4.0 | 5.0 | 11.1 |

## 全局属性

`<footer>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<footer>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置 \<footer> 样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    footer {
      text-align: center;
      padding: 3px;
      background-color: DarkSalmon;
      color: white;
    }
  </style>
</head>
<body>
  <footer>
    <p>Author: Hello World<br>
    <a href="mailto:hello@example.com">hello@example.com</a></p>
  </footer>
</body>
</html>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<footer>` 元素：

```css
footer {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg