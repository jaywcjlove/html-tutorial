HTML onpaste 事件属性
===

## 示例

在 \<input> 元素中粘贴一些文本时执行 JavaScript：

\<input type="text" onpaste="myFunction()" value="Paste something in here">


## 定义和使用

当用户在元素中粘贴一些内容时，`onpaste` 属性会触发。

**注意：** 尽管所有 HTML 元素都支持 `onpaste` 属性，但实际上不可能将某些内容粘贴到例如 \<p> 元素中，除非该元素已将 contenteditable 设置为“true”（请参阅 下面的“更多示例”）。

**提示：** `onpaste` 属性主要用于 type="text" 的 \<input> 元素。

**提示：** 可以通过三种方式在元素中粘贴一些内容：

* 按 CTRL + V
* 从浏览器的编辑菜单中选择“粘贴”
* 右键单击显示上下文菜单并选择“粘贴”命令

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onpaste | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onpaste="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | The script to be run on onpaste |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

在 \<p> 元素中粘贴一些文本时执行 JavaScript（注意 [contenteditable](../attribute/contenteditable.md) 设置为“true”）：

```html
<p contenteditable="true" onpaste="myFunction()">尝试在本段中粘贴一些内容。</p>
```

```html idoc:preview:iframe
<p contenteditable="true" onpaste="myFunction()">尝试在本段中粘贴一些内容。</p>

<script>
function myFunction() {
  alert("You pasted text!");
}
</script>
```


## 相关页面

HTML 参考: [oncopy 事件](./oncopy.md)

HTML 参考: [oncut 事件](./oncut.md)

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

