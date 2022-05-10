HTML oncopy 事件属性
===

## 示例

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

## 定义和使用

`oncopy` 属性在用户复制元素的内容时触发。

**提示：** 当用户复制使用 [\<img>](../tags/img.md) 元素创建的元素（例如图像）时，也会触发 `oncopy` 属性。

**提示：** `oncopy` 属性主要用于 type="text" 的 [\<input>](../tags/input.md) 元素。

**提示：** 复制元素/元素内容的三种方式：

* 按 CTRL + C
* 从浏览器的编辑菜单中选择“复制”
* 右键单击显示上下文菜单并选择“复制”命令

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oncopy | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** 在尝试复制图像时，oncopy 属性在某些浏览器中可能无法正常工作（请参阅下面的“更多示例”）。

## 语法

```html
<element oncopy="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 oncopy 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

### 示例

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


### 示例

复制图像时执行 JavaScript：

```html
<img src="../assets/chrome.svg" oncopy="myFunction()">
```

```html idoc:preview:iframe
尝试复制下面的图像（右键单击图像并选择“复制图像”）。<br>
<img src="../assets/chrome.svg" oncopy="myFunction()" alt="Chrome" width="120" height="120">

<p><strong>注意：</strong>此示例在某些浏览器中可能无法按预期工作。</p>
<script>
  function myFunction() {
    alert("你复制了图片！");
  }
</script>
```