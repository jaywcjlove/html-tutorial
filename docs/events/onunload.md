HTML onunload 事件属性
===

## 示例

当用户卸载文档时执行 JavaScript：

```html idoc:preview:iframe
<body onunload="myFunction()">
  <p>关闭此窗口或按 F5 重新加载页面。</p>
  <p><strong>注意：</strong>由于不同的浏览器设置，此事件可能并不总是按预期工作。</p>
  <script>
    function myFunction() {
      alert("感谢您访问文档！");
    }
  </script>

</body>
```

```html
<body onunload="myFunction()">
```

## 定义和使用

一旦页面卸载（或浏览器窗口已关闭），`onunload` 属性就会触发。

`onunload` 发生在用户离开页面时（通过单击链接、提交表单、关闭浏览器窗口等）

**注意：** 如果重新加载页面，也会触发 `onunload` 事件（以及 [onload](./onload.md) 事件）。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onunload | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** 由于不同的浏览器设置，此事件可能并不总是按预期工作。

## 语法

```html
<element onunload="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onunload 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

