HTML \<input type="color">
===

## 示例

显示一个颜色选择器（具有预定义的红色值）：

```html idoc:preview:iframe
<label for="favcolor">Select your favorite color:</label>
<input type="color" id="favcolor" name="favcolor" value="#ff0000">
```

## 定义和用法

`<input type="color">` 定义了一个颜色选择器。

默认值为 `#000000`（黑色）。 该值必须采用七个字符的十六进制表示法。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="color" | 20.0 | 38.0 | 29.0 | 10.1 | 11.01 |


## 语法

```html
<input type="color">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg