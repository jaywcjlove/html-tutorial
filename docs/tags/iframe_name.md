HTML \<iframe> name 属性
===

## 示例

用作链接目标的 \<iframe>：

```html idoc:preview:iframe
<iframe
  src="iframe.html"
  name="iframe_a"
  width="100%"
>
</iframe>
<br>
<a
  href="./a.html"
  target="iframe_a"
>
点击，iframe 加载 &lt;a&gt; 文档
</a>
```

## 定义和用法

`name` 属性指定 iframe 的名称。

此 `name` 属性可用于引用 JavaScript 中的元素，或用作 `<a>` 或 `<form>` 元素的 `target` 属性的值，或 ` 的 `formtarget` 属性 <input>` 或 `<button>` 元素。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| name      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<iframe name="name">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *name* | 指定 \<iframe> 的名称 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
