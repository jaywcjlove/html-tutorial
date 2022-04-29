HTML \<datalist> Tag
===

## 示例

具有预定义选项的数据列表（连接到 \<input> 元素）：

```html idoc:preview
<label for="browser">Choose your browser from the list:</label>
<input list="browsers" name="browser" id="browser">

<datalist id="browsers">
  <option value="Edge">
  <option value="Firefox">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

## 定义和用法

`<datalist>` 标签指定了一个 [\<input>](./input.md) 元素的预定义选项列表。

`<datalist>` 标签用于为 [\<input>](./input.md) 元素提供“自动完成”功能。 用户在输入数据时将看到一个预定义选项的下拉列表。

`<datalist>` 元素的 id 属性必须等于 [\<input>](./input.md) 元素的 list 属性（这将它们绑定在一起）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<datalist> | 20.0 | 10.0 | 4.0 | 12.1 | 9.5 |

## 全局属性

`<datalist>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<datalist>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<datalist>` 元素：

```css
datalist {
  display: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg