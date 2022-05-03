HTML disabled 属性
===

## 定义和用法

`disabled` 属性是一个布尔属性。

当存在时，它指定元素应该被禁用。

禁用的元素不可用。

可以设置 `disabled` 属性以阻止用户使用该元素，直到满足某些其他条件（例如选择复选框等）。 然后，JavaScript 可以删除禁用的值，并使元素再次可用。

## 适用于

`disabled` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<button>](../tags/button.md)     | [disabled](../tags/button_disabled.md)   |
| [\<fieldset>](../tags/fieldset.md) | [disabled](../tags/fieldset_disabled.md) |
| [\<input>](../tags/input.md)       | [disabled](../tags/input_disabled.md)    |
| [\<optgroup>](../tags/optgroup.md) | [disabled](../tags/optgroup_disabled.md) |
| [\<option>](../tags/option.md)     | [disabled](../tags/option_disabled.md)   |
| [\<select>](../tags/select.md)     | [disabled](../tags/select_disabled.md)   |
| [\<textarea>](../tags/textarea.md) | [disabled](../tags/textarea_disabled.md) |

## 示例

### Button 示例

禁用的按钮：

```html idoc:preview:iframe
<button type="button" disabled>Click Me!</button>
```

### Fieldset 示例

禁用一组相关的表单元素：

```html idoc:preview:iframe
<fieldset disabled>
  <legend>Personalia:</legend>
  Name: <input type="text"><br>
  Email: <input type="text"><br>
  Date of birth: <input type="text">
</fieldset>
```

### Input 示例

带有禁用输入字段的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname" disabled><br>
  <input type="submit" value="Submit">
</form>
```

### Optgroup 示例

禁用的选项组：

```html idoc:preview:iframe
<select>
  <optgroup label="German Cars" disabled>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```

### Option 示例

带有一个禁用选项的下拉列表：

```html idoc:preview:iframe
<select>
  <option value="volvo" disabled>Volvo</option>
  <option value="saab">Saab</option>
  <option value="vw">VW</option>
  <option value="audi">Audi</option>
</select>
```

### Select 示例

禁用的下拉列表：

```html idoc:preview:iframe
<select disabled>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="mercedes">Mercedes</option>
  <option value="audi">Audi</option>
</select>
```

### Textarea 示例

禁用的文本 textarea：

```html idoc:preview:iframe
<textarea disabled>
在 HTML Tutorial，您将学习如何制作网站。 他们提供所有 Web 开发技术的免费教程。
</textarea>
```

## 浏览器支持

`disabled` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<button>](../tags/button.md)     | Yes | Yes           | Yes | Yes | Yes |
| [\<fieldset>](../tags/fieldset.md) | Yes | ❌ 不支持 | Yes | 7.0 | Yes |
| [\<input>](../tags/input.md)       | 1.0 | 6.0           | 1.0 | 1.0 | 1.0 |
| [\<optgroup>](../tags/optgroup.md) | 1.0 | 8.0           | Yes | Yes | Yes |
| [\<option>](../tags/option.md)     | 1.0 | 8.0           | 1.0 | Yes | Yes |
| [\<select>](../tags/select.md)     | Yes | Yes           | Yes | Yes | Yes |
| [\<textarea>](../tags/textarea.md) | Yes | Yes           | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
