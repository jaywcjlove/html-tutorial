HTML \<meter> 标签
===

## 示例

使用仪表元素测量给定范围内的数据（仪表）：

```html idoc:preview
<label for="disk_c">Disk usage C:</label>
<meter id="disk_c" value="2" min="0" max="10">2 out of 10</meter><br>

<label for="disk_d">Disk usage D:</label>
<meter id="disk_d" value="0.6">60%</meter>
```

## 定义和用法

`<meter>` 标签定义了已知范围内的标量测量值，或小数值。 这也称为量规。

示例：磁盘使用情况、查询结果的相关性等。

**注意：** `<meter>` 标签不应用于指示进度（如在进度条中）。 对于进度条，使用 [\<progress>](./progress.md) 标签。

**提示：** 始终添加 [\<label>](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<meter> | 8.0 | 13.0 | 16.0 | 6.0 | 11.5 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [form](./meter_form.md)       | *form\_id* | 指定 \<meter> 元素属于哪种形式 |
| [high](./meter_high.md)       | *number*   | 指定被认为是高值的范围 |
| [low](./meter_low.md)         | *number*   | 指定被认为是低值的范围 |
| [max](./meter_max.md)         | *number*   | 指定范围的最大值 |
| [min](./meter_min.md)         | *number*   | 指定范围的最小值。 默认值为 0 |
| [optimum](./meter_optimum.md) | *number*   | 指定仪表的最佳值是什么值 |
| [value](./meter_value.md)     | *number*   | 必需的。 指定仪表的当前值 |

## 全局属性

`<meter>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<meter>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg