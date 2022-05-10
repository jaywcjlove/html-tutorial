HTML onafterprint 事件属性
===

## 示例

当页面开始打印或打印对话框已关闭时执行 JavaScript：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body onafterprint="myFunction()">
  <h2>尝试打印此文档</h2>
  <p>提示：键盘快捷键，例如 Ctrl+P 设置要打印的页面。</p>
  <p>注意： Safari 和 Opera 不支持 onafterprint 事件。</p>
  <p>注意：在 IE 中，onafterprint 事件发生在打印对话框之前，而不是之后。</p>
  <script>
  function myFunction() {
    alert("该文件正在打印中");
  }
  </script>
</body>
</html>
```

```html
<body onafterprint="myFunction()">
```

## 定义和使用

`onafterprint` 属性在页面开始打印或打印对话框已关闭时触发。

**提示：** `onafterprint` 属性通常与 [onbeforeprint](./onbeforeprint.md) 属性一起使用。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| `onafterprint` | 63 | Yes | Yes | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** 在 IE/Edge 中，`onafterprint` 属性出现在打印对话框之前，而不是之后。

## 语法

```html
<element onafterprint="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onafterprint 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | \<body> |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
