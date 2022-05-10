HTML oncut 事件属性
===

当用户剪切元素的内容时触发

## 示例

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

## 定义和使用

`oncut` 属性在用户剪切元素的内容时触发。

**注意：** 虽然所有 HTML 元素都支持 `oncut` 属性，但实际上不可能剪切例如 [\<p>](../tags/p.md) 元素的内容，除非该元素已将 [contenteditable](../attribute/contenteditable.md) 设置为“true”（请参阅 下面的“更多示例”）。

**提示：** `oncut` 属性主要用于 type="text" 的 [\<input>](../tags/input.md) 元素。

**提示：** 剪切元素内容的三种方式：

* 按 CTRL + X
* 从浏览器的编辑菜单中选择“剪切”
* 右键单击显示上下文菜单并选择“剪切”命令

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oncut | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element oncut="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `oncut` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

在剪切 \<p> 元素的某些文本时执行 JavaScript（注意 [contenteditable](../attribute/contenteditable.md) 设置为“true”）：

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


## 相关页面

HTML 参考: [oncopy 事件](./oncopy.md)

HTML 参考: [onpaste 事件](./onpaste.md)



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


