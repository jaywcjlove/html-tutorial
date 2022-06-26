HTML oncut 属性
===

## 定义和用法

`oncut` 属性在用户剪切元素内容时触发。

**注意：** 虽然所有 HTML 元素都支持 `oncut` 属性，但实际上不可能剪切例如 `<p>` 元素的内容，除非该元素设置了 `contenteditable` 属性为“true”（参见下面的“更多示例”）。

**提示：** 剪切元素内容的三种方式：

* 按 <kbd>CTRL</kbd> + <kbd>X</kbd>
* 从浏览器的编辑菜单中选择“剪切”
* 右键单击显示上下文菜单并选择“剪切”命令

## 适用于

`oncut` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [oncut](../events/oncut.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Input 示例

在 \<input> 元素中剪切一些文本时执行 JavaScript：

```html
<input type="text" oncut="myFunction()" value="尝试剪切此文本">
```

```html idoc:preview:iframe
<input type="text" oncut="myFunction()" value="尝试剪切此文本">

<p id="demo"></p>

<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "你剪了文字！";
}
</script>
```

### P 示例

在剪切 \<p> 元素的某些文本时执行 JavaScript（注意 `contenteditable` 设置为 `true`）：

```html
<p contenteditable="true" oncut="myFunction()">尝试剪切此文本</p>
```

```html idoc:preview:iframe
<p contenteditable="true" oncut="myFunction()">尝试剪切此文本</p>

<script>
function myFunction() {
  alert("你剪了文字！");
}
</script>
```

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oncut           | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

