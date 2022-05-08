HTML \<iframe> srcdoc 属性
===

## 示例

带有 `srcdoc` 属性的 \<iframe>：

```html idoc:preview:iframe
<iframe
  srcdoc="<p>Hello world!</p>"
  src="iframe.html"
>
</iframe>
```

## 定义和使用

`srcdoc` 属性指定要在内联框架中显示的页面的 HTML 内容。

**提示：** 此属性应与 `sandbox` 和 `seamless` 属性一起使用。

如果浏览器支持 `srcdoc` 属性，它将覆盖 `src` 属性（如果存在）中指定的内容。

如果浏览器不支持 `srcdoc` 属性，它将显示在 `src` 属性中指定的文件（如果存在）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| srcdoc    | 20.0 | 79.0 | 25.0 | 6.0 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<iframe srcdoc="HTML_code">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *HTML\_code* | 要在 iframe 中显示的 HTML 内容。 必须是有效的 HTML 语法 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

