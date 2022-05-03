HTML low 属性
===

## 定义和用法

`low` 属性指定仪表的值被认为是低值的范围。

`low` 属性值必须大于 [`min`](./min.md) 属性值，也必须小于 [`high`](./high.md) 和 [`max`](./max.md) 属性值。

## 适用于

`low` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<meter>](../tags/meter.md) | [low](../tags/meter_low.md) |

## 示例

具有当前值和最小、最大、高和低段的仪表：

```html idoc:preview:iframe
<meter min="0" low="40" high="90" max="100" value="95"></meter>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| low       | 8.0 | ❌ 不支持 | 6.0 | 6.0 | 11.0 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg