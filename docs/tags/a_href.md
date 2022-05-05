HTML `<a>` 标签的 href 属性
===

## 示例

`href` 属性指定链接的目的地：

```html idoc:preview
<a target="_blank" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

## 定义和用法

`href` 属性指定链接到的页面的 URL。

如果 `href` 属性不存在，则 [`<a>`](./a.md) 标记将不是超链接。

**提示：** 您可以使用 `href="#top"` 或 `href="#"` 链接到当前页面的顶部！

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| href      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<a href="URL">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| *URL* | 链接的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `href="http://www.example.com/default.htm"`）<br>* 相对 URL - 指向网站内的文件（如 `href="default.htm"`）<br>* 链接到页面内具有指定 id 的元素（如 `href="#section2"`）<br>* 其他协议（如 `https://`、`ftp://`、`mailto:`、`file:` 等）<br>* 一个脚本（比如 `href="javascript:alert('Hello');"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

如何使用图片作为链接：

```html idoc:preview
<a href="https://github.com/jaywcjlove/html-tutorial">
  <img
    alt="HTML Tutorial"
    width="100" height="100"
    src="https://avatars1.githubusercontent.com/u/1680273?s=460&v=4">
</a>
```

如何链接到电子邮件地址：

```html idoc:preview
<a href="mailto:someone@example.com">Send email</a>
```

如何链接到电话号码：

```html idoc:preview
<a href="tel:+4733378901">+47 333 78 901</a>
```

如何链接到同一页面上的另一个部分：

```html idoc:preview
<a href="#更多示例">跳转到 #更多示例</a>
```

如何链接到 JavaScript：

```html idoc:preview
<a href="javascript:alert('Hello World!');">执行 JavaScript</a>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg