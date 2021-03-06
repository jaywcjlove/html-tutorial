HTML \<img> usemap 属性
===

## 示例

带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="A 超链接文档" href="a.htm">
  <area shape="rect" coords="290,172,333,250" alt="Img 文档" href="img.htm">
  <area shape="circle" coords="337,300,44" alt="Div 文档" href="div.htm">
</map>
```

## 定义和用法

`usemap` 属性将图像指定为客户端图像映射（图像映射是具有可点击区域的图像）。

`usemap` 属性与 `<map>` 元素的 name 属性相关联，并在 `<img>` 和 `<map>` 之间创建关系。

**注意：** 如果 `<img>` 元素是 `<a>` 或 `<button>` 元素的后代，则不能使用 `usemap` 属性。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| usemap    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img usemap="#mapname">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *#mapname* | 哈希字符 (`#`) 加上要使用的 \<map> 元素的名称 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg