HTML maxlength 属性
===

## 定义和用法

`maxlength` 属性指定元素中允许的最大字符数。

## 适用于

`maxlength` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md)       | [maxlength](../tags/input_maxlength.md)    |
| [\<textarea>](../tags/textarea.md) | [maxlength](../tags/textarea_maxlength.md) |

## 示例

### Input 示例

最大长度为 10 个字符的 [\<input>](../tags/input.md) 元素：

```html idoc:preview:iframe
<form action="/action_page.php">
  Username: <input type="text" name="usrname" maxlength="10"><br>
  <input type="submit" value="Submit">
</form>
```

### Textarea 示例

最大长度为 50 个字符的文本区域：

```html idoc:preview:iframe
<textarea maxlength="50">
在这里输入文本...
</textarea>
```

## 浏览器支持

`maxlength` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<input>](../tags/input.md)       | 1.0 | 2.0  | 1.0 | 1.0 | 1.0  |
| [\<textarea>](../tags/textarea.md) | Yes | 10.0 | 4.0 | Yes | 15.0 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
