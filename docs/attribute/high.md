HTML high 属性
===

## 定义和用法

`high` 属性指定仪表的值被认为是高值的范围。

`high` 属性值必须小于 `max` 属性值，也必须大于 `low` 和 `min` 属性值。

## 适用于

`high` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<meter>](../tags/meter.md) | [high](../tags/meter_high.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

具有当前值和最小、最大、高和低段的仪表：

```html idoc:preview:iframe
<meter min="0" low="40" high="90" max="100" value="65"></meter>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| high      | 8.0 | ❌ 不支持 | 6.0 | 6.0 | 11.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg