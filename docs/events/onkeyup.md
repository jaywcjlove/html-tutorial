HTML onkeyup 事件属性
===

## 示例

当用户释放键时执行 JavaScript：

```html idoc:preview:iframe
当用户在输入字段中释放一个键时触发一个函数。 该函数将字符转换为大写。<br>
输入你的名字：<input type="text" id="fname" onkeyup="myFunction()">
<script>
  function myFunction() {
    var x = document.getElementById("fname");
    x.value = x.value.toUpperCase();
  }
</script>
```

```html
<input type="text" onkeyup="myFunction()">
```

## 定义和使用

`onkeyup` 属性在用户释放一个键（在键盘上）时触发。

**提示：** `onkeyup` 事件相关的事件顺序：

1. [onkeydown](ev_onkeydown.asp)
2. [onkeypress](ev_onkeypress.asp)
3. onkeyup

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onkeyup | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onkeyup="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `onkeyup` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: [\<base>](../tags/base.md), [\<bdo>](../tags/bdo.md), [\<br>](../tags/br.md), [\<head>](../tags/head.md), [\<html>](../tags/html.md), [\<iframe>](../tags/iframe.md), [\<meta>](../tags/meta.md), [\<param>](../tags/param.md), [\<script>](../tags/script.md), [\<style>](../tags/style.md), 和 [\<title>](../tags/title.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

将 `onkeydown` 与`onkeyup` 属性一起使用：

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

```html
<input type="text" onkeydown="keydownFunction()" onkeyup="keyupFunction()">
```

## 示例

输出在文本字段中释放的实际键：

```html idoc:preview:iframe
当用户在输入字段中释放一个键时触发一个函数。 该函数输出在文本字段内释放的实际键/字母。<br>
输入你的名字：<input type="text" id="fname" onkeyup="myFunction()">
<p>我的名字是：<span id="demo"></span></p>

<script>
  function myFunction() {
    var x = document.getElementById("fname").value;
    document.getElementById("demo").innerHTML = x;
  }
</script>
```



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

