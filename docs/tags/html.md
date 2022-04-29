HTML \<html> Tag
===

## 示例

一个简单的 HTML 文档：

```html idoc:preview:iframe
<!DOCTYPE html>
<html lang="en">
<head>
  <title>文件标题</title>
</head>
<body>
  <h1>这是一个标题</h1>
  <p>这是一个段落。</p>
</body>
</html>
```

## 定义和用法

`<html>` 标签表示 HTML 文档的根。

`<html>` 标记是所有其他 HTML 元素的容器（[\<!DOCTYPE>](./doctype.md) 标记除外）。

**注意：** 您应该始终在 `<html>` 标记中包含 [lang](../attribute/global/lang.md) 属性，以声明网页的语言。 这是为了帮助搜索引擎和浏览器。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<html> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [xmlns](./html_xmlns.md) | https://www.w3.org/1999/xhtml | 指定 XML 命名空间属性（如果您需要您的内容符合 XHTML） |

## 全局属性

`<html>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 相关页面

HTML 教程: [HTML Introduction](../tutorial/intro.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<form>` 元素：

```css
html {
  display: block;
}
html:focus {
  outline: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg