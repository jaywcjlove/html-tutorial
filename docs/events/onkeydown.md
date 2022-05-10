HTML onkeydown 事件属性
===

当用户按下某个键时触发

## 示例

当用户按键时执行 JavaScript：

```html idoc:preview:iframe
当用户在输入框中按下一个键时会触发一个函数。<br>
<input type="text" onkeydown="myFunction(this)"><br>
执行 onkeydown 事件：<span id="info"> </span>
<script>
function myFunction(evn) {
  document.getElementById('info').innerHTML = '您在输入框中按下了一个键!';
}
</script>
```

```html
<input type="text" onkeydown="myFunction()">
```

## 定义和使用

`onkeydown` 属性在用户按下一个键（在键盘上）时触发。

**提示：** `onkeydown` 事件相关的事件顺序：

1. onkeydown
2. [onkeypress](./onkeypress.md)
3. [onkeyup](./onkeyup.md)

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onkeydown | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onkeydown="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onkeydown 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: [\<base>](../tags/base.md), [\<bdo>](../tags/bdo.md), [\<br>](../tags/br.md), [\<head>](../tags/head.md), [\<html>](../tags/html.md), [\<iframe>](../tags/iframe.md), [\<meta>](../tags/meta.md), [\<param>](../tags/param.md), [\<script>](../tags/script.md), [\<style>](../tags/style.md), 和 [\<title>](../tags/title.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

将 `onkeydown` 与 `onkeyup` 属性一起使用：

```html idoc:preview:iframe
<input type="text" id="demo" onkeydown="keydownFunction()" onkeyup="keyupFunction()">

<script>
function keydownFunction() {
  document.getElementById("demo").style.backgroundColor = "red";
}

function keyupFunction() {
  document.getElementById("demo").style.backgroundColor = "green";
}
</script>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


