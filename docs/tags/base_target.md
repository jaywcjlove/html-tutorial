HTML \<base> target 属性
===

## 示例

为页面上的所有超链接和表单指定默认目标：

```html idoc:preview:iframe
<head>
  <base href="https://wangchujiang.com/" target="_blank">
</head>
<body>
  <div>
    <a href="html-tutorial/tags/head.html">HTML base Tag</a> 注意，这个超链接，将在新窗口打开 ”https://wangchujiang.com/html-tutorial/tags/head.html“ </div>
</body>
```

## 定义和用法

`target` 属性指定页面中所有超链接和表单的默认目标。

此属性可以通过使用每个超链接/表单的“目标”属性来覆盖。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| target    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<base target="_blank|_self|_parent|_top">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| \_blank  | 在新窗口或选项卡中打开链接 |
| \_self   | 默认。 在单击时在同一框架中打开链接 |
| \_parent | 在父框架中打开链接 |
| \_top    | 在整个窗口中打开链接 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg