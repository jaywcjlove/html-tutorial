HTML onreset 事件属性
===

单击表单中的重置按钮时触发

## 示例

单击表单中的重置按钮时执行 JavaScript：

```html idoc:preview:iframe
当您重置表单时，会触发一个提醒某些文本的功能。
<form onreset="myFunction()">
  输入名字: <input type="text">
  <input type="reset">
</form>
<script>
  function myFunction() {
    alert("The form was reset");
  }
</script>
```

```html
<form onreset="myFunction()">
  输入名称: <input type="text">
  <input type="reset">
</form>
```

## 定义和使用

`onreset` 属性在表单被重置时触发。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onreset | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onreset="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `onreset` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | \<form> |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


