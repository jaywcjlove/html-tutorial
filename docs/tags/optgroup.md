HTML \<optgroup> 标签
===

## 示例

使用 \<optgroup> 标签对相关选项进行分组：

```html idoc:preview:iframe
<label for="cars">Choose a car:</label>
<select  name="cars" id="cars">
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

## 定义和用法

`<optgroup>` 标签用于在 [\<select>](./select.md) 元素（下拉列表）中对相关选项进行分组。

如果您有很长的选项列表，则用户更容易处理相关选项组。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<optgroup> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [disabled](./optgroup_disabled.md) | disabled | 指定应禁用选项组 |
| [label](./optgroup_label.md)       | *text*   | 指定选项组的标签 |

## 全局属性

`<optgroup>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<optgroup>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg