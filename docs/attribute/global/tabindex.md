HTML `tabindex` 属性
===

指定元素的 tab 键顺序（当“tab”键用于导航）

## 实例

带有指定 tab 键顺序的链接：

```html idoc:preview
<a href="https://www.w3schools.com/" tabindex="2">W3Schools</a>
<a href="http://www.google.com/" tabindex="1">Google</a>
<a href="http://www.microsoft.com/" tabindex="3">Microsoft</a>
```

## 定义和使用

`tabindex` 属性指定元素的 tab 键顺序（当“tab”按钮用于导航时）。

`tabindex` 属性可用于任何 HTML 元素（它将验证任何 HTML 元素。但是，它不一定有用）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;tabindex&gt;__ | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<element tabindex="number">
```

## 属性值

值 Value | 描述 Description
---- | ----
number | 规定元素的 `tab` 键控制次序（1 是第一个）。

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg