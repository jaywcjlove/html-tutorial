HTML `hidden` 属性
===

指定一个元素尚不相关或不再相关。

## 实例

隐藏段落：

```html idoc:preview
👇👇👇👇👇 下面段落被隐藏了，点击显示源码，查看实例
<p hidden>This paragraph should be hidden.</p>
```

## 定义和使用

`hidden` 属性是一个布尔属性。

当存在时，它指定一个元素尚不相关或不再相关。

浏览器不应显示指定了 `hidden` 属性的元素。

`hidden` 属性也可以用来防止用户看到一个元素，直到满足其他一些条件（比如选择一个复选框等）。 然后，JavaScript 可以删除 hidden 属性，并使元素可见。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;hidden&gt;__ | 6.0 | 11.0 | 4.0 | 5.1 | 11.1 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element hidden>
```


[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg