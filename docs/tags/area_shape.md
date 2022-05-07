HTML \<area> shape 属性
===

## 示例

使用 `shape` 属性指定图像映射中每个区域的形状：

```html idoc:preview
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="a.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```
<!--rehype:style=min-height: 280px;-->

## 定义和用法

`shape` 属性指定区域的形状。

`shape` 属性与 `coords` 属性一起使用来指定区域的大小、形状和位置。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| shape     | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<area shape="default|rect|circle|poly">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| default | Specifies the entire region  |
| rect    | Defines a rectangular region |
| circle  | Defines a circular region    |
| poly    | Defines a polygonal region   |
