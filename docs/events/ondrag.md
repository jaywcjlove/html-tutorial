HTML ondrag 事件属性
===

拖动元素时运行的脚本

## 示例

在拖动 \<p> 元素时执行 JavaScript：

```html
<p draggable="true" ondrag="myFunction(event)">拖我一把！</p>
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

## 定义和使用

`ondrag` 属性在拖动元素或文本选择时触发。

拖放是 HTML5 中非常常见的功能。 当您“抓住”一个对象并将其拖到不同的位置时。 有关更多信息，请参阅我们关于 [HTML5 拖放](../tutorial/draganddrop.md) 的 HTML 教程。

**注意：** 要使元素可拖动，请使用全局 HTML5 [draggable](../attribute/draggable.md) 属性。

**提示：** 链接和图片默认是可拖动的，不需要 `draggable` 属性。

在拖放操作的不同阶段使用并可能发生许多事件属性：

- **在可拖动目标上触发的事件**（源元素）：
  * [ondragstart](./ondragstart.md) - 当用户开始拖动元素时触发
  * ondrag - 拖动元素时触发
  * [ondragend](./ondragend.md) - 当用户完成拖动元素时触发
- **在放置目标上触发的事件：**
  * [ondragenter](./ondragenter.md) - 当拖动的元素进入放置目标时触发
  * [ondragover](./ondragover.md) - 当被拖动的元素在放置目标上方时触发
  * [ondragleave](./ondragleave.md) - 当被拖动的元素离开放置目标时触发
  * [ondrop](./ondrop.md) - 当拖动的元素被放置在放置目标上时触发

**注意：** 拖动元素时，ondrag 事件每 350 毫秒触发一次。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| ondrag | 4.0 | 9.0 | 3.5 | 6.0 | 12.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element ondrag="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `ondrag` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 相关页面

HTML 教程: [HTML5 拖放](../tutorial/draganddrop.md)

HTML 参考: [HTML draggable 属性](../attribute/draggable.md)



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

