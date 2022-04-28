HTML contenteditable 属性
===

## 实例

一段可编辑的段落：

```html idoc:preview:iframe
<p contenteditable="true">这是一个可编辑的段落。</p>
```

## 定义和使用

`contenteditable` 属性指定元素的内容是否可编辑。

⚠️ 注意：当元素上没有设置 `contenteditable` 属性时，该元素将从其父元素继承它。

## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;contenteditable&gt;__ | 4.0 | 6.0 | 3.5 | 3.1 | 10.1

## 语法

```html
<element contenteditable="true|false">
```

## 属性值

值 Value | 描述 Description
---- | ----
true | 指定元素是可编辑的
false | 指定元素不可编辑

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg