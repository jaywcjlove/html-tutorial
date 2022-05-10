HTML onkeypress 事件属性
===

当用户按下某个键时触发

## 示例

当用户按键时执行 JavaScript：

```html idoc:preview:iframe
<input type="text" onkeypress="myFunction()">
<script>
  function myFunction() {
    alert("您在输入字段中按下了一个键");
  }
</script>
```

```html
<input type="text" onkeypress="displayResult()">
```

## 定义和使用

`onkeypress` 属性在用户按下一个键（在键盘上）时触发。

**提示：** onkeypress 事件相关的事件顺序：

1. [onkeydown](./onkeydown.md)
2. onkeypress
3. [onkeyup](./onkeyup.md)

**注意：** 并非所有浏览器中的所有键（例如 ALT、CTRL、SHIFT、ESC）都会触发 `onkeypress` 事件。 要仅检测用户是否按下了某个键，请改用 [onkeydown](./onkeydown.md)，因为它适用于所有键。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| `onkeypress` | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onkeypress="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `onkeypress` 上运行的脚本 |
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


