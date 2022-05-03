HTML id 属性
===

## 定义和用法

`id` 属性为 HTML 元素指定一个唯一的 id（该值在 HTML 文档中必须是唯一的）。

`id` 属性最常用于指向样式表中的样式，并通过 JavaScript（通过 HTML DOM）来操作具有特定 id 的元素。

## 适用于

`id` 属性是一个 [全局属性](../reference/standardattributes.md)，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 全部 [HTML](../tags/README.md) 元素 | [id](./global/id.md) |

## 示例

使用 id 属性通过 JavaScript 操作文本：

```html idoc:preview:iframe
<html>
<body>
  <h1 id="myHeader">Hello World!</h1>
  <button onclick="displayResult()">Change text</button>
  <script>
    function displayResult() {
      document.getElementById("myHeader").innerHTML = "Have a nice day!";
    }
  </script>
</body>
</html>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| id        | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg