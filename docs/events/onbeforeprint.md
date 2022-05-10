HTML onbeforeprint 事件属性
===

在打印文档之前运行的脚本

## 示例

在即将打印页面时执行 JavaScript：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body onbeforeprint="myFunction()">

<h1>尝试打印此文档</h1>
<p><b>提示：</b> 键盘快捷键，例如 Ctrl+P 设置要打印的页面。</p>
<p><b>注意：</b> Safari 和 Opera 不支持 onbeforeprint 事件。</p>

<script>
function myFunction() {
  alert("您即将打印此文档！");
}
</script>

</body>
</html>

```

```html
<body onbeforeprint="myFunction()">
```

## 定义和使用

`onbeforeprint` 属性在即将打印页面时触发（在打印对话框出现之前）。

**提示：** `onbeforeprint` 属性通常与 [onafterprint](./onafterprint.md) 属性一起使用。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onbeforeprint   | 63 | Yes | Yes | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<element onbeforeprint="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onbeforeprint 上运行的脚本 |

## Technical Details

| Supported HTML tags: | \<body> |
| --- | --- |
