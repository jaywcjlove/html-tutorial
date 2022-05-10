HTML onmouseup 事件属性
===

当在元素上释放鼠标按钮时触发

## 示例

在段落上释放鼠标按钮时执行 JavaScript：

```html idoc:preview:iframe
<p id="p1" onmousedown="mouseDown()" onmouseup="mouseUp()">点击文字！ mouseDown() 函数在鼠标按钮在此段落上按下时触发。 该函数将文本的颜色设置为红色。 mouseUp() 函数在释放鼠标按钮时触发。 mouseUp() 函数将文本的颜色设置为绿色。
</p>
<script>
  function mouseDown() {
    document.getElementById("p1").style.color = "red";
  }
  function mouseUp() {
    document.getElementById("p1").style.color = "green";
  }
</script>
```

```html
<p onmouseup="mouseUp()">点击文字！</p>
```

## 定义和使用

当在元素上释放鼠标按钮时会触发 onmouseup 属性。

**提示：** onmouseup 事件相关的事件顺序（针对鼠标左键/中键）：

1.  [onmousedown](./onmousedown.md)
2.  onmouseup
3.  [onclick](./onclick.md)

onmouseup 事件相关的事件顺序（针对鼠标右键）：

1.  [onmousedown](./onmousedown.md)
2.  onmouseup
3.  [oncontextmenu](./oncontextmenu.md)

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onmouseup       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onmouseup="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 onmouseup 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: [\<base>](../tags/base.md), [\<bdo>](../tags/bdo.md), [\<br>](../tags/br.md), [\<head>](../tags/head.md), [\<html>](../tags/html.md), [\<iframe>](../tags/iframe.md), [\<meta>](../tags/meta.md), [\<param>](../tags/param.md), [\<script>](../tags/script.md), [\<style>](../tags/style.md), 和 [\<title>](../tags/title.md) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


