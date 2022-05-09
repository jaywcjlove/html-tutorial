HTML hidden 属性
===

## 定义和用法

`hidden` 属性是一个布尔属性。

当存在时，它指定一个元素尚不相关或不再相关。

浏览器不应显示指定了 `hidden` 属性的元素。

`hidden` 属性也可以用来阻止用户看到一个元素，直到满足其他一些条件（比如选择一个复选框等）。 然后，JavaScript 可以删除 hidden 属性，并使元素可见。

## 适用于

`hidden` 属性是一个 [全局属性](../reference/standardattributes.md)，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 全部 [HTML](../tags/README.md) 元素 | [hidden](./global/hidden.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

隐藏段落：

```html idoc:preview:iframe
<p hidden>这一段应该被隐藏。</p>
上面一段文本被隐藏了。
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| hidden    | 6.0 | 11.0 | 4.0 | 5.1  | 11.1 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg