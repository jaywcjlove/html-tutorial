HTML onblur 属性
===

## 定义和用法

`onblur` 属性会在元素失去焦点时触发。

Onblur 最常与表单验证代码一起使用（例如，当用户离开表单字段时）。

**提示：** `onblur` 属性与 `onfocus` 属性相反。

## 适用于

`onblur` 属性是 [事件属性](../reference/eventattributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [onblur](../attribute/onblur.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

当用户离开时验证输入字段：

```html idoc:preview:iframe
输入你的名字： <input type="text" name="fname" id="fname" onblur="myFunction()">
<p>当您离开输入字段时，会触发一个函数，将输入文本转换为大写。</p>

<script>
  function myFunction() {
    var x = document.getElementById("fname");
    x.value = x.value.toUpperCase();
  }
</script>
```

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onblur | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

