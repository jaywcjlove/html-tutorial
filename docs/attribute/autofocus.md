HTML autofocus 属性
===

## 定义和用法

`autofocus` 属性是一个布尔属性。

当存在时，它指定元素在页面加载时应该自动获得焦点。

## 适用于

`autofocus` 属性可用于以下元素：

| 标签 Element | 属性 Attribute |
| ----- | ----- |
| [\<button>](../tags/button.md)     | [autofocus](../tags/button_autofocus.md)   |
| [\<input>](../tags/input.md)       | [autofocus](../tags/input_autofocus.md)    |
| [\<select>](../tags/select.md)     | [autofocus](../tags/select_autofocus.md)   |
| [\<textarea>](../tags/textarea.md) | [autofocus](../tags/textarea_autofocus.md) |

## 示例

### Button 示例

带自动对焦的按钮：

```html idoc:preview:iframe
<button type="button" autofocus>Click Me!</button>
```

### Input 示例

让 “名” 输入字段在页面加载时自动获得焦点：

```html idoc:preview:iframe
<form action="/action_page.php">
  名: <input type="text" name="fname" autofocus><br>
  姓: <input type="text" name="lname"><br>
  <input type="submit">
</form>
```

### Textarea 示例

具有自动对焦的文本区域：

```html idoc:preview:iframe
<textarea autofocus>
我们提供所有 Web 开发技术的免费教程。
</textarea>
```

## 浏览器支持

`autofocus` 属性对每个元素都有以下浏览器支持：

| 标签 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| form     | 5.0 | 10.0 | 4.0 | 5.0 | 9.6 |
| input    | 5.0 | 10.0 | 4.0 | 5.0 | 9.6 |
| textarea | Yes | 10.0 | 4.0 | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg