HTML oncopy 属性
===

## 定义和用法

`oncopy` 属性在用户复制元素内容时触发。

**提示：** 当用户复制使用 `<img>` 元素创建的元素（例如图像）时，也会触发 `oncopy` 属性。

**提示：** `oncopy` 属性主要用于具有 `type="text"` 的 `<input>` 元素。

**提示：** 复制元素/元素内容的三种方式：

* 按 <kbd>CTRL</kbd> + <kbd>C</kbd>
* 从浏览器的编辑菜单中选择“复制”
* 右键单击显示上下文菜单并选择“复制”命令

## 适用于

`oncopy` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [oncopy](../events/oncopy.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Input 示例

在复制 \<input> 元素的某些文本时执行 JavaScript：

```html
<input type="text" oncopy="myFunction()" value="尝试复制此文本">
```

```html idoc:preview:iframe
<input type="text" oncopy="myFunction()" value="尝试复制此文本">

<p id="demo"></p>

<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "你复制了文字！"
}
</script>
```

### P 示例

在复制 \<p> 元素的某些文本时执行 JavaScript：

```html
<p oncopy="myFunction()">尝试复制此文本</p>
```

```html idoc:preview:iframe
<p oncopy="myFunction()">尝试复制此文本</p>

<script>
function myFunction() {
  alert("你复制了文字！");
}
</script>
```

### Img 示例

复制图像时执行 JavaScript：

```html
<img src="xxx.gif" oncopy="myFunction()">
```

```html idoc:preview:iframe
<p>尝试复制下面的图像（右键单击图像并选择“复制图像”）。</p>

<img src="../assets/editors-001.png" oncopy="myFunction()" alt="editors image" height="150">

<p><strong>笔记：</strong> 此示例在某些浏览器中可能无法按预期工作。</p>

<script>
function myFunction() {
  alert("你复制了图片！");
}
</script>
```

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oncopy          | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** 在尝试复制图像时，oncopy 属性在某些浏览器中可能无法正常工作（参见上面的示例）。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


