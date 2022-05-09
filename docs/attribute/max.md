HTML max 属性
===

## 定义和用法

`max` 属性指定元素的最大值。

当被 `<progress>` 元素使用时，`max` 属性指定任务总共需要多少工作。

## 适用于

`max` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md)       | [max](../tags/input_max.md)    |
| [\<meter>](../tags/meter.md)       | [max](../tags/meter_max.md)    |
| [\<progress>](../tags/progress.md) | [max](../tags/progress_max.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

使用 [min](./min.md) 和 max 属性：

```html idoc:preview:iframe
<form action="/action_page.php">
  Enter a date before 1980-01-01:
  <input type="date" name="bday" max="1979-12-31"><br/>
  Enter a date after 2000-01-01:
  <input type="date" name="bday" min="2000-01-02"><br/>
  Quantity (between 1 and 5):
  <input type="number" name="quantity" min="1" max="5"><br/>
  <input type="submit">
</form>
```

### Meter 示例

具有当前值和最小[min](./min.md)、最大、高和低段的仪表：

```html idoc:preview:iframe
<meter min="0" low="40" high="90" max="100" value="95"></meter>
```

### Progress 示例

正在下载：

```html idoc:preview:iframe
<progress value="22" max="100"></progress>
```

## 浏览器支持

`max` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<input>](../tags/input.md)       | 5.0 | 10.0      | 16.0 | 5.1 | 10.6 |
| [\<meter>](../tags/meter.md)       | 8.0 | ❌ 不支持  | 6.0  | 6.0 | 11.0 |
| [\<progress>](../tags/progress.md) | 8.0 | 10.0      | 16.0 | 6.0 | 11.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg