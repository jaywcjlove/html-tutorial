HTML onerror 事件属性
===

## 示例

如果加载图像时发生错误，则执行 JavaScript：

```html idoc:preview:iframe
<img src="image.gif" onerror="myFunction()">

<p>如果加载图像时发生错误，则会触发一个函数。 该函数显示一个带有文本的警告框。 在这个例子中，我们引用了一个不存在的图像，因此会发生 onerror 事件。</p>
<div id="info" style="color: red;"> </div>
<script>
function myFunction() {
  document.getElementById('info').innerHTML = '无法加载图像。'
}
</script>
```

```html
<img src="image.gif" onerror="myFunction()">
```

## 定义和使用

`onerror` 属性在加载外部文件（例如文档或图像）时发生错误时触发。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onerror | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->
## 语法

```html
<element onerror="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `onerror` 上运行的脚本 |

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | \<img>, \<input type="image">, \<object>, \<link>, \<script> |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

