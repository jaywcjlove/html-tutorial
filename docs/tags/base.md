HTML \<base> 标签
===

 标记指定文档中所有相对 URL 的基本 URL 和/或目标

## 示例

为页面上的所有链接指定默认 URL 和默认目标：

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

`<base>` 标记指定文档中所有相对 URL 的基本 URL 和/或目标。

`<base>` 标记必须具有 href 或 target 属性，或两者兼有。

文档中只能有一个 `<base>` 元素，并且它必须在 \<head> 元素内。


## Browser Support

| Element |  ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<base> | Yes | Yes | Yes | Yes | Yes |

## 属性 idoc:preview

| 属性 Attribute | 值 Value | 描述 Description |
| ------ | ------ | ------ |
| [href](./base_href.md)     | *URL*                         | 指定页面中所有相对 URL 的基本 URL|
| [target](./base_target.md) | \_blank<br/> \_parent<br/>\_self<br/>\_top | 指定页面中所有超链接和表单的默认目标|


## 全局属性

`<base>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<base>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg