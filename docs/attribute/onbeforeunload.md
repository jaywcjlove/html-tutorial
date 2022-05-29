HTML onbeforeunload 属性
===

## 定义和用法

`onbeforeunload` 事件在文档即将被卸载时触发。

此事件允许您在确认对话框中显示一条消息，以通知用户他/她是要留下还是离开当前页面。

确认框中显示的默认消息在不同的浏览器中有所不同。 但是，标准消息类似于“您确定要离开此页面吗？”。 您无法删除此消息。

但是，您可以将自定义消息与默认消息一起编写。 请参阅此页面上的第一个示例。

**注意：** 在 Firefox 中，只会显示默认消息（不是自定义消息（如果有））。

## 适用于

`onbeforeunload` 属性是 [Event Attributes](../attribute/onbeforeunload.md) 的一部分，可用于以下元素：

| 元素 | 事件 |
| --- | --- |
| [\<body>](../tags/body.md) | [onbeforeunload](../attribute/onbeforeunload.md) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


## 示例

当页面即将被卸载时执行 JavaScript：

```html idoc:preview:iframe
<body onbeforeunload="return myFunction()">
<p>关闭此窗口，按 F5 或单击下面的链接以调用 onbeforeunload 事件。</p>

<a href="https://jaywcjlove.github.io/html-tutorial">单击此处访问 https://jaywcjlove.github.io/html-tutorial</a>
  
<script>
  function myFunction() {
    return "在这里写一些聪明的东西......";
  }
</script>
</body>
```

## 浏览器支持

表中的数字指定了完全支持该事件的第一个浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onbeforeunload  | Yes | Yes | Yes | Yes | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

