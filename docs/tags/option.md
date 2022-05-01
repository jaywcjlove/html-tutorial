HTML \<option> Tag
===

## 示例

包含四个选项的下拉列表：

```html idoc:preview:iframe
<label for="cars">Choose a car:</label>
<select id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```
<!--rehype:style=height: 60px;-->

## 定义和用法

`<option>` 标签在选择列表中定义一个选项。

`<option>` 元素进入 [\<select>](./select.md)、[\<optgroup>](./optgroup.md) 或 [\<datalist>](./datalist.md) 元素。

**注意：** `<option>` 标签可以不带任何属性使用，但您通常需要 **value** 属性，该属性指示表单提交时发送到服务器的内容。

**提示：** 如果您有很长的选项列表，您可以在 [\<optgroup>](./optgroup.md) 标记中对相关选项进行分组。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<option> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [disabled](./option_disabled.md) | disabled | 指定一个选项应该被禁用 |
| [label](./option_label.md)       | *text*   | 为选项指定较短的标签 |
| [selected](./option_selected.md) | selected | 指定在页面加载时应预先选择一个选项 |
| [value](./option_value.md)       | *text*   | 指定要发送到服务器的值 |

## 全局属性

`<option>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<option>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

在 \<datalist> 元素中使用 \<option>：

```html idoc:preview:iframe
<label for="browser">从列表中选择您的浏览器：</label>
<input list="browsers" name="browser" id="browser">

<datalist id="browsers">
  <option value="Edge">
  <option value="Firefox">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```
<!--rehype:style=height: 60px;-->

在 \<optgroup> 元素中使用 \<option>：

```html idoc:preview:iframe
<label for="cars">Choose a car:</label>
<select id="cars">
  <optgroup label="Swedish Cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```
<!--rehype:style=height: 60px;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg