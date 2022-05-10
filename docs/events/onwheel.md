HTML onwheel 事件属性
===

当鼠标滚轮在元素上向上或向下滚动时触发

## 示例

当用户在 [\<div>](../tags/div.md) 元素上滚动鼠标滚轮时执行 JavaScript：

```html
<div onwheel="myFunction()">在我身上滚动鼠标滚轮</div>
```

```html idoc:preview:iframe
<style>
#myDIV {
  border: 1px solid black;
}
</style>
<div id="myDIV" onwheel="myFunction()">此示例演示如何将“onwheel”事件分配给 DIV 元素。 在我身上滚动鼠标滚轮 - 向上或向下！</div>
<p>当您在 div 上滚动鼠标滚轮时会触发一个函数。 该函数将 div 的字体大小设置为 35 像素。</p>
<p><strong>注意：</strong>Internet Explorer 或 Safari 不支持 onwheel 事件。</p>
<script>
  function myFunction() {
    document.getElementById("myDIV").style.fontSize = "35px";
  }
</script>
```

## 定义和使用

当指针设备的滚轮在元素上向上或向下滚动时，onwheel 属性会触发。

当用户使用触摸板（如笔记本电脑的“鼠标”）滚动或缩放元素时，onwheel 属性也会触发。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onwheel | 31.0 | 9.0 | 17.0 | ❌ 不支持 | 18.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onwheel="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 `onwheel` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


