HTML ondblclick 属性
===

## 定义和用法

`ondblclick` 属性在鼠标双击元素时触发。

## 适用于

`ondblclick` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [ondblclick](../events/ondblclick.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Button 示例

双击按钮时执行 JavaScript：

```html
<button ondblclick="myFunction()">双击我</button>
```

```html idoc:preview:iframe
<button ondblclick="myFunction()">双击我</button>

<p id="demo"></p>

<p>双击按钮时触发一个函数。 该函数在 id="demo" 的 p 元素中输出一些文本。</p>

<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Hello World";
}
</script>
```

### P 示例

双击 \<p> 元素将其文本颜色更改为红色：

```html
<p id="demo" ondblclick="myFunction()">双击我以更改我的文本颜色。</p>

<script>
function myFunction() {
  document.getElementById("demo").style.color = "red";
}
</script>
```

```html idoc:preview:iframe
<p id="demo" ondblclick="myFunction()">双击我以更改我的文本颜色。</p>

<script>
function myFunction() {
  document.getElementById("demo").style.color = "red";
}
</script>
```

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| ondblclick      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
