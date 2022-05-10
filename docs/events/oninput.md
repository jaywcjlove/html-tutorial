HTML oninput 事件属性
===

当元素获得用户输入时运行的脚本

## 示例

当用户在 \<input> 字段中写入内容时执行 JavaScript：

```html idoc:preview:iframe
<input type="text" id="myInput" oninput="myFunction()">
<p id="demo"></p>
<script>
function myFunction() {
  var x = document.getElementById("myInput").value;
  document.getElementById("demo").innerHTML = "你写了: " + x;
}
</script>
```

```html
<input type="text" oninput="myFunction()">
```

## 定义和使用

`oninput` 属性在元素获得用户输入时触发。

当 [\<input>](../tags/input.md) 或 [\<textarea>](../tags/textarea.md) 元素的值更改时，`oninput` 属性会触发。

**提示：** 此事件类似于 [onchange](./onchange.md) 事件。 不同之处在于，`oninput` 事件在元素的值发生更改后立即发生，而 `onchange` 在元素失去焦点时发生。 另一个区别是 `onchange` 事件也适用于 [\<select>](../tags/select.md) 元素。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oninput         | Yes | 9.0 | 4.0 | 5.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element oninput="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 oninput 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<input type="password">](../tags/input_type_password.md), [\<input type="search">](../tags/input_type_search.md), [\<input type="text">](../tags/input_type_text.md) 和 [\<textarea>](../tags/textarea.md) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

