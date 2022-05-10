HTML onsubmit 事件属性
===

提交表单时触发

## 示例

提交表单时执行 JavaScript：

```html idoc:preview:iframe
<form action="/action_page.php" onsubmit="myFunction()">
  输入名字: <input type="text" name="fname">
  <input type="submit" value="Submit">
</form>

<script>
function myFunction() {
  alert("表格已提交");
}
</script>
```

```html
<form onsubmit="myFunction()">
  输入名字: <input type="text">
  <input type="submit">
</form>
```

## 定义和使用

`onsubmit` 属性在提交表单时触发。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onsubmit | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<form onsubmit="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onsubmit 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<form>](../tags/form.md) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

