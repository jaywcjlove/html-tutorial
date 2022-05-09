HTML \<map> 标签
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

`<map>` 标签用于定义图像映射。 图像地图是具有可点击区域的图像。

`<map>` 元素的必需名称属性与 [\<img>](./img.md) 的 usemap 属性相关联，并在图像和地图之间创建关系。

`<map>` 元素包含许多 [\<area>](./area.md) 元素，它们定义了图像地图中的可点击区域。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<map>  | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [name](./map_name.md) | *mapname* | 必需的。 指定图像映射的名称 |

## 全局属性

`<map>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<map>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

另一个带有可点击区域的图像地图：

```html idoc:preview:iframe
<img src="../assets/workplace.jpg" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126" href="sun.htm" alt="Sun">
  <area shape="circle" coords="90,58,3" href="mercur.htm" alt="Mercury">
  <area shape="circle" coords="124,58,8" href="venus.htm" alt="Venus">
</map>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<map>` 元素：

```css
map {
  display: inline;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg