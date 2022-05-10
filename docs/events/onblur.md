HTML onblur 事件属性
===

在元素失去焦点时触发

## 示例

当用户离开时验证输入字段：

```html idoc:preview:iframe
输入你的名字: <input type="text" name="fname" id="fname" onblur="myFunction()">
<p>当您离开输入字段时，会触发一个函数，将输入文本转换为大写。</p>
<script>
function myFunction() {
  var x = document.getElementById("fname");
  x.value = x.value.toUpperCase();
}
</script>
```

```html
<input type="text" name="fname" id="fname" onblur="myFunction()">
```

## 定义和使用

`onblur` 属性会在元素失去焦点时触发。

`onblur` 最常与表单验证代码一起使用（例如，当用户离开表单字段时）。

**提示：** onblur 属性与 [onfocus](./onfocus.md) 属性相反。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onblur | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onblur="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onblur 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: \<base>, \<bdo>, \<br>, \<head>, \<html>, \<iframe>, \<meta>, \<param>, \<script>, \<style>, \<title> |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

将 `onblur` 与 `onfocus` 属性一起使用：

```html idoc:preview:iframe
<p>当您输入输入字段时，会触发将背景颜色设置为黄色的功能。 当您离开输入字段时，会触发一个函数，将背景颜色设置为红色。</p>
输入你的名字：<input type="text" id="myInput" onfocus="focusFunction()" onblur="blurFunction()">
<script>
  // 焦点 = 将输入的背景颜色更改为黄色
  function focusFunction() {
    document.getElementById("myInput").style.background = "yellow";
  }
  // 无焦点 = 将输入的背景颜色更改为红色
  function blurFunction() {
    document.getElementById("myInput").style.background = "red";
  }
</script>
```

```html
<input type="text" onfocus="focusFunction()" onblur="blurFunction()">
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

