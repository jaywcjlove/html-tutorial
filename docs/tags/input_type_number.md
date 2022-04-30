HTML \<input type="number">
===

## 示例

定义一个用于输入数字的字段（您还可以设置接受哪些数字的限制）：

```html idoc:preview:iframe
<label for="quantity">Quantity (between 1 and 5):</label>
<input type="number" id="quantity" name="quantity" min="1" max="5">
```

## 定义和用法

`<input type="number">` 定义了一个用于输入数字的字段。

使用以下属性来指定限制：

* [max](./input_max.md) - 指定允许的最大值
* [min](./input_min.md) - 指定允许的最小值
* [step](./input_step.md) - 指定合法数字区间
* [value](./input_value.md) - 指定默认值

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="number" | 25.0 | 12.0 | Not supported | Not supported | 10.1 |

## 语法

```html
<input type="number">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg