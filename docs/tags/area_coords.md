HTML \<area> coords 属性
===

## 示例

使用 `coords` 属性指定图像映射中每个区域的坐标：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126" href="a.html" alt="Sun">
  <area shape="circle" coords="90,58,3" href="address.html" alt="Mercury">
  <area shape="circle" coords="124,58,8" href="applet.html" alt="Venus">
</map>
```

## 定义和用法

`coords` 属性指定图像地图中某个区域的坐标。

`coords` 属性与 `shape` 属性一起使用来指定区域的大小、形状和位置。

**提示：** 区域左上角的坐标为 `0,0`。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| coords    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area coords="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *x1,y1,x2,y2*          | 指定矩形左上角和右下角的坐标（shape="rect"） |
| *x,y,radius*           | 指定圆心坐标和半径（shape="circle"） |
| *x1,y1,x2,y2,..,xn,yn* | 指定多边形边缘的坐标。 如果第一个和最后一个坐标对不相同，浏览器会添加最后一个坐标对来闭合多边形（shape="poly") |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg