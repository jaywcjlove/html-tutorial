HTML dirname 属性
===

## 定义和用法

`dirname` 属性启用输入字段/文本区域的文本方向的提交

`dirname` 属性的值始终是输入字段/文本区域的名称，后跟“.dir”。

## 适用于

`dirname` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md)       | [dirname](../tags/input_dirname.md)    |
| [\<textarea>](../tags/textarea.md) | [dirname](../tags/textarea_dirname.md) |

## 示例

### Input 示例

将提交字段文本方向的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  First name: <input type="text" name="fname" dirname="fname.dir">
  <input type="submit" value="Submit">
</form>
```

### Textarea 示例

将提交字段文本方向的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  Text:
  <textarea name="explanation" dirname="explanation.dir"></textarea>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

`dirname` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [input](../tags/input.md)    | Yes | No | No | Yes | Yes |
| [textarea](../tags/textarea.md) | Yes | No | No | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
