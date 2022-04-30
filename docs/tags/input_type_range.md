HTML \<input type="range">
===

## 示例

单选按钮让用户只选择有限数量的选项之一：

```html idoc:preview:iframe
<label for="points">Points (between 0 and 10):</label>
<input type="range" id="points" name="points" min="0" max="10">
```

## 定义和用法

`<input type="range">` 定义了一个用于输入精确值不重要的数字的控件（如滑块控件）。

默认范围是 0 到 100。但是，您可以使用以下属性设置接受哪些数字的限制。

* [max](./input_max.md) - 指定允许的最大值
* [min](./input_min.md) - 指定允许的最小值
* [step](./input_step.md) - 指定合法数字区间
* [value](./input_value.md) - 指定默认值

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="range" | 4.0 | 10.0 | 23.0 | 3.1 | 10.1 |

## 语法

```html
<input type="range">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg