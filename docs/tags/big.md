HTML \<big> 标签
===

[![](https://shields.io/badge/HTML5-已废弃-yellow?logo=HTML5)](https://caniuse.com/?search=<big>)

## HTML5 不支持

`<big>` 标签在 HTML 4 中用于定义更大的文本。

## 改用什么？

为 HTML 元素指定不同的字体大小（使用 CSS）：

```html idoc:preview:iframe
<html>
<head>
  <style>
    p.ex1 {
      font-size: 30px;
    }
    p.ex2 {
      font-size: 50px;
    }
  </style>
</head>
<body>
  <p>This is a normal paragraph.</p>
  <p class="ex1">This is a bigger paragraph.</p>
  <p class="ex2">This is a much bigger paragraph.</p>
</body>
</html>
```