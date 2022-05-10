HTML onfocus 事件属性
===

## 示例

当输入字段获得焦点时执行 JavaScript：

```html idoc:preview:iframe
<p>当输入字段之一获得焦点时触发一个函数。 该函数更改输入字段的背景颜色。</p>
名: <input type="text" id="fname" onfocus="myFunction(this.id)"><br>
姓: <input type="text" id="lname" onfocus="myFunction(this.id)">

<script>
function myFunction(x) {
  document.getElementById(x).style.background = "yellow";
}
</script>
```

```html
<input type="text" id="fname" onfocus="myFunction(this.id)">
```

## 定义和使用

`onfocus` 属性在元素获得焦点时触发。

`onfocus` 最常与 [\<input>](../tags/input.md)、[\<select>](../tags/select.md) 和 [\<a>](../tags/a.md) 一起使用。

**提示：** `onfocus` 属性与 [onblur](./onblur.md) 属性相反。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onfocus         | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onfocus="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 onfocus 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: \<base>, \<bdo>, \<br>, \<head>, \<html>, \<iframe>, \<meta>, \<param>, \<script>, \<style>, and \<title> |

## 更多示例

将 `onblur` 与 `onfocus` 属性一起使用：

```html idoc:preview:iframe
<p>当您输入输入字段时，会触发将背景颜色设置为黄色的功能。 当您离开输入字段时，会触发一个函数，将背景颜色设置为红色。</p>
输入你的名字: <input type="text" id="myInput" onfocus="focusFunction()" onblur="blurFunction()">

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
