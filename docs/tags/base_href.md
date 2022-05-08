HTML \<base> href 属性
===

## 示例

为页面上的所有相对 URL 指定一个基本 URL：

```html idoc:preview:iframe
<head>
  <base href="https://wangchujiang.com/" target="_blank">
</head>
<body>
  <img src="html-tutorial/assets/chrome.svg" width="24" height="39" alt="chrome"> 请注意，我们只为图像指定了一个相对地址。 由于我们在 head 部分指定了基本 URL，浏览器将在“https://wangchujiang.com/html-tutorial/assets/chrome.svg”中查找图像。
  <div>
    <a href="html-tutorial/tags/head.html">HTML base Tag</a> 注意，这个超链接，将在新窗口打开 ”https://wangchujiang.com/html-tutorial/tags/head.html“
  </div>
</body>
```

## 定义和用法

`href` 属性指定页面上所有相对 URL 的基本 URL。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| href      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<base href="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 充当基本 URL 的绝对 URL（如“http://www.example.com/”） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg