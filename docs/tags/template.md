HTML \<template> 标签
===

## 示例

使用 \<template> 保存一些在页面加载时将被隐藏的内容。 使用 JavaScript 显示它：

```html idoc:preview:iframe
<button onclick="showContent()">Show hidden content</button>
<template>
  <h2>Flower</h2>
  <img src="../assets/example.png" width="214">
</template>
<script>
  function showContent() {
    var temp = document.getElementsByTagName("template")[0];
    var clon = temp.content.cloneNode(true);
    document.body.appendChild(clon);
  }
</script>
```

## 定义和用法

`<template>` 标签用作一个容器，用于在页面加载时保存一些对用户隐藏的 HTML 内容。

`<template>` 中的内容可以稍后使用 JavaScript 渲染。

如果您有一些 HTML 代码要反复使用，则可以使用 `<template>` 标签，但在您要求之前不要使用。 要做到这一点*没有* `<template>` 标签，您必须使用 JavaScript 创建 HTML 代码，以防止浏览器呈现代码。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<template> | 26.0 | 13.0 | 22.0 | 8.0 | 15.0 |

## 全局属性

`<template>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 更多示例

用一个新的 div 元素为数组中的每个项目填充网页。 每个 div 元素的 HTML 代码都在模板元素内：

```html idoc:preview:iframe
<button onclick="showContent()">Show hidden content</button>
<template>
  <div class="myClass">I like: </div>
</template>
<script>
  var myArr = ["Audi", "BMW", "Ford", "Honda", "Jaguar", "Nissan"];
  function showContent() {
    var temp, item, a, i;
    temp = document.getElementsByTagName("template")[0];
    item = temp.content.querySelector("div");
    for (i = 0; i < myArr.length; i++) {
      a = document.importNode(item, true);
      a.textContent += myArr[i];
      document.body.appendChild(a);
    }
  }
</script>
```
<!--rehype:style=height: 130px;-->

检查浏览器对 \<template> 的支持：

```html idoc:preview:iframe
<script>
if (document.createElement("template").content) {
  document.write("Your browser supports template!");
} else {
  document.write("Your browser does not supports template!");
}
</script>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg