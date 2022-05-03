HTML min 属性
===

## 定义和用法

`min` 属性指定元素元素的最小值。

当与 [`<meter>`](../tags/meter.md) 元素一起使用时，`min` 属性指定仪表的下限。

## 适用于

`min` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<input>](../tags/input.md) | [min](../tags/input_min.md) |
| [\<meter>](../tags/meter.md) | [min](../tags/meter_min.md) |

## 示例

### Input 示例

使用 [min](./min.md) 和 [max](./max.md) 属性：

```html idoc:preview:iframe
<form action="/action_page.php">
  Enter a date before 1980-01-01:
  <input type="date" name="bday" max="1979-12-31"><br>
  Enter a date after 2000-01-01:
  <input type="date" name="bday" min="2000-01-02"><br>
  Quantity (between 1 and 5):
  <input type="number" name="quantity" min="1" max="5"><br>

  <input type="submit">

</form>
```

### Meter 示例

具有当前值和[min](./min.md)、[max](./max.md)、[high](./high.md)和 [low](./low.md)的仪表：

```html idoc:preview:iframe
<meter min="0" low="40" high="90" max="100" value="95"></meter>
```

## 浏览器支持

`min` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| input   | 5.0 | 10.0 | 16.0 | 5.1 | 10.6 |
| meter   | 5.0 | 10.0 | 16.0 | 5.1 | 10.6 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg