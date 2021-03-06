HTML \<!DOCTYPE> 声明
===

```html
<!DOCTYPE html>
<html>
<head>
<title>文档标题</title>
</head>

<body>
文档内容......
</body>

</html>
```

## 定义和使用

所有 HTML 文档都必须以 `<!DOCTYPE>` 声明开头。

声明不是 HTML 标签。 对于浏览器来说，这是一个关于预期文档类型的“信息”。

在 HTML 5 中，声明很简单：

```html
<!DOCTYPE html>
```

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __\<!DOCTYPE>__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 较旧的 HTML 文档

在旧文档（HTML 4 或 XHTML）中，声明更复杂，因为声明必须引用 DTD（文档类型定义）。

HTML 4.01:

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

XHTML 1.1:

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```

## HTML 元素和文档类型

查看[我们所有 HTML 元素的表格](../reference/dtd.md)，以及每个元素出现在什么 Doctype 中。

## 提示和注意事项

提示：`<!DOCTYPE>` 声明不区分大小写。

## Examples

```html
<!DOCTYPE html>
<!DocType html>
<!Doctype html>
<!doctype html>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg