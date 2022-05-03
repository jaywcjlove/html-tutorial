HTML class 属性
===

## 定义和用法

`class` 属性为元素指定一个或多个类名。

`class` 属性主要用于指向样式表中的类。 但是，JavaScript 也可以使用它（通过 HTML DOM）来更改具有指定类的 HTML 元素。

## 适用于

`class` 属性是 [全局属性](../reference/standardattributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 所有 HTML 元素 | [class](att_global_class.asp) |

## 示例

在 HTML 文档中使用 class 属性：

```html idoc:preview:iframe
<html>
<head>
  <style>
    h1.intro {
      color: blue;
    }

    p.important {
      color: green;
    }
  </style>
</head>
<body>
  <h1 class="intro">标题 1</h1>
  <p>一个段落。</p>
  <p class="important">请注意，这是一个重要的段落。 :)</p>
</body>
</html>
```
<!--rehype:style=height: 200px;-->

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| class     | Yes | Yes | Yes | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
