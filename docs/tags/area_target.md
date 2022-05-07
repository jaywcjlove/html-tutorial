HTML \<area> target 属性
===

## 示例

使用 target 属性指定在图像映射中打开链接文档的位置：

```html idoc:preview
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area target="_blank" shape="rect" coords="34,44,270,350" alt="Computer" href="a.html">
  <area target="_blank" shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area target="_blank" shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```
<!--rehype:style=min-height: 280px;-->

## 定义和用法

`target` 属性指定打开链接文档的位置。

仅在存在 `href` 属性时使用。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| target    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area target="_blank|_self|_parent|_top|framename">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| \_blank     | 在新窗口或选项卡中打开链接的文档 |
| \_self      | 在单击时在同一框架中打开链接的文档 |
| \_parent    | 在父框架中打开链接的文档 |
| \_top       | 在整个窗口中打开链接的文档 |
| *framename* | 在命名的 iframe 中打开链接的文档 |<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg