HTML ondrag 属性
===

## 定义和用法

拖动元素或文本选择时会触发 `ondrag` 属性。

要了解拖放，请阅读我们关于 [HTML5 拖放](../tutorial/draganddrop.md) 的 HTML 教程。

**提示：** 链接和图片默认可拖动，不需要 [`draggable`](../attribute/draggable.md) 属性。

在拖放操作的不同阶段使用并可能发生许多事件属性：

* **在可拖动目标上触发的事件**（源元素）**：**

  * [`ondragstart`](./ondragstart.md) - 当用户开始拖动元素时触发
  * [`ondrag`](./ondrag.md) - 拖动元素时触发
  * [`ondragend`](./ondragend.md) - 当用户完成拖动元素时触发

* **在放置目标上触发的事件：**

  * [`ondragenter`](./ondragenter.md) - 当被拖动的元素进入放置目标时触发
  * [`ondragover`](./ondragover.md) - 当拖动的元素在放置目标上方时触发
  * [`ondragleave`](./ondragleave.md) - 当被拖动的元素离开放置目标时触发
  * [`ondrop`](./ondrop.md) - 当被拖动的元素放在放置目标上时触发

**注意：** 拖动元素时，`ondrag` 事件每 350 毫秒触发一次。

## 适用于

`ondrag` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [ondrag](../events/ondrag.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

在拖动 \<p> 元素时执行 JavaScript：

```html
<p draggable="true" ondrag="myFunction(event)">Drag me!\</p>
```


```html idoc:preview:iframe
<style>
  .droptarget {
    float: left; 
    width: 100px; 
    height: 35px;
    margin: 15px;
    padding: 10px;
    border: 1px solid #aaaaaa;
  }
</style>
<p>在两个矩形之间来回拖动 p 元素：</p>

<div class="droptarget" ondrop="drop(event)" ondragover="allowDrop(event)">
  <p ondragstart="dragStart(event)" ondrag="dragging(event)" draggable="true" id="dragtarget">拖我一把！</p>
</div>
<div class="droptarget" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
<p style="clear:both;" id="demo"></p>
<script>
  function dragStart(event) {
    event.dataTransfer.setData("Text", event.target.id);
  }

  function dragging(event) {
    document.getElementById("demo").innerHTML = "p 元素被拖动";
  }

  function allowDrop(event) {
    event.preventDefault();
  }

  function drop(event) {
    event.preventDefault();
    var data = event.dataTransfer.getData("Text");
    event.target.appendChild(document.getElementById(data));
    document.getElementById("demo").innerHTML = "p 元素被删除";
  }
</script>
```

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| ondrag          | 4.0 | 9.0 | 3.5 | 6.0 | 12.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
