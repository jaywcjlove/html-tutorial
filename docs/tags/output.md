HTML \<output> 标签
===

## 示例

执行计算并在 \<output> 元素中显示结果：

```html idoc:preview:iframe
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" value="50">
  +<input type="number" id="b" value="25">
  =<output name="x" for="a b"></output>
</form>
```

## 定义和用法

`<output>` 标签用于表示计算的结果（如脚本执行的计算）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<output> | 10.0 | 13.0  | 4.0 | 5.1 | 11.0 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [for](./output_for.md)   | *element\_id* | 指定计算结果与计算中使用的元素之间的关系|
| [form](./output_form.md) | *form\_id*    | 指定输出元素属于哪个表单|
| [name](./output_name.md) | *name*        | 指定输出元素的名称|

## 全局属性

`<output>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<output>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<output>` 元素：

```css
output {
  display: inline;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg