HTML \<bdo> dir 属性
===

## 示例

指定文本方向：

```html idoc:preview
<p>Hello world. <bdo dir="rtl">Hello world</bdo></p>
```

## 定义和用法

必需的 `dir` 属性指定 `<bdo>` 元素内文本的文本方向。

## 浏览器支持

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| dir       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<bdo dir="ltr|rtl">
```

## 属性值

| 值 Value | 描述 Description |
| -------- | ------ |
| ltr   | 从左到右的文本方向 |
| rtl   | 从右到左的文本方向 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg