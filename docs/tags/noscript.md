HTML \<noscript> 标签
===

## 示例

\<noscript> 标签的使用：

```html idoc:preview:iframe
<script>
  document.write("Hello World!")
</script>
<noscript>Your browser does not support JavaScript!</noscript>
```

## 定义和用法

`<noscript>` 标记定义了要显示给在浏览器中禁用脚本或浏览器不支持脚本的用户的替代内容。

`<noscript>` 元素可以在 [\<head>](./head.md) 和 [\<body>](./body.md) 中使用。 在 [\<head>](./head.md) 中使用时，`<noscript>` 元素只能包含 [\<link>](./link.md)、[\<style>](./style.md) 和 [\<meta>](./meta.md) 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<noscript> | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<noscript>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。


## 相关页面

HTML 教程: [HTML Scripts](../tutorial/scripts.md)
