HTML onselect 事件属性
===

## 示例

在 \<input> 元素中选择了一些文本后执行 JavaScript：

```html idoc:preview:iframe
一些文字：<input type="text" value="Select me!!" onselect="myFunction()">

<p>当在输入字段中选择了一些文本时，会触发函数 myFunction()。 该函数显示一条消息。</p>

<script>
function myFunction() {
  alert("您选择了一些文本！");
}
</script>
```

```html
<input type="text" onselect="myFunction()" value="Hello world!">
```

## 定义和使用

`onselect` 属性在元素中的某些文本被选中后触发。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onselect | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onselect="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `onselect` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<input type="file">](../tags/input_type_file.md), [\<input type="password">](../tags/input_type_password.md), [\<input type="text">](../tags/input_type_text.md), 和 [\<textarea>](../tags/textarea.md) |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


