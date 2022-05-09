HTML class 属性
===

主要用于指向样式表中的类。

## 实例

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

<h1 class="intro">Header 1</h1>
<p>A paragraph.</p>
<p class="important">Note that this is an important paragraph. :)</p>

</body>
</html>
```

## 定义和使用

`class` 属性为元素指定一个或多个类名。

`class` 属性主要用于指向样式表中的类。 但是，JavaScript 也可以使用它（通过 HTML DOM）来更改具有指定类的 HTML 元素。

## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;class&gt;__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```HTML
<element class="classname">
```

## 属性值

值 Value | 描述 Description
---- | ----
classname | 为元素指定一个或多个类名。 要指定多个类，请用空格分隔类名，例如 `<span class="left important"`>。 这允许您为一个 HTML元素组合多个 CSS 类。<br />命名规则：<br /> 1. 必须以字母 A-Z 或 a-z 开头<br />2. 后面可以跟：字母 (A-Za-z)、数字 (0-9)、连字符 ("-") 和下划线 ("_")
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

向一个 HTML 元素添加多个类：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <style>
    h1.intro { color: blue; text-align: center; }
    .important { background-color: yellow; }
  </style>
</head>
<body>

<h1 class="intro important">Header 1</h1>
<p>A paragraph.</p>

</body>
</html>
```

使用 JavaScript 为第一个带有 `class="example"`（索引 0）的元素添加黄色(yellow)背景色。

```html idoc:preview:iframe
<div class="example">Hello World!<div>
<script>
var x = document.getElementsByClassName("example");
x[0].style.backgroundColor = "yellow";
</script>
```

使用 JavaScript 将 `mystyle` 类添加到 `id="myDIV"` 的元素中：

document.getElementById("myDIV").classList.add("mystyle");

```html idoc:preview:iframe
<style>.mystyle {color: red;}</style>
<div id="myDIV">Hello World!<div>
<script>
document.getElementById("myDIV").classList.add("mystyle");
</script>
```

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg