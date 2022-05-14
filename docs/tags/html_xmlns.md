HTML \<html> xmlns 属性
===

## 示例

一个简单的 XHTML 文档，具有最少的必需标签：

```html idoc:preview:iframe
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <title>Title of the document</title>
</head>

<body>
  文本内容......
</body>

</html>
```

## 定义和用法

`xmlns` 属性指定文档的 `xml` 命名空间。

**注意：** `xmlns` 属性在 `XHTML` 中是必需的，在 `HTML 4.01` 中无效，在 `HTML5` 中是可选的。

**注意：** 当 `XHTML` 文档中缺少 `xmlns` 属性时，`<http://w3.org>` 上的 HTML 验证器不会报错。 这是因为命名空间 `xmlns=http://www.w3.org/1999/xhtml` 是默认的，即使你不包含它也会被添加到 `<html>` 标签中。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| xmlns     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<html xmlns="http://www.w3.org/1999/xhtml">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| http://www.w3.org/1999/xhtml | 要使用的名称空间（用于 XHTML 文档） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

