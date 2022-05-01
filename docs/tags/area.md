HTML \<area> 标签
===

## 示例

带有可点击区域的图像地图，点击下面`电脑`，`咖啡`和`手机`，进入不同的页面：

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

`<area>` 标签定义了图像映射中的一个区域（图像映射是具有可点击区域的图像）。

`<area>` 元素总是嵌套在 `<map>` 标签内。

**注意：** `<img>` 中的 `usemap` 属性与 `<map>` 元素的 `name` 属性相关联，并在图像和地图之间建立关系。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __\<area>__ | Yes | Yes | Yes | Yes | Yes |

## 属性

| 属性 Attribute | 值 Value | 描述 Description |
| ----- | ----- | ----- |
| [alt](./area_alt.md)                      | *text* | 指定区域的替代文本。 如果存在 href 属性，则为必需 |
| [coords](./area_coords.md)                | *coordinates* | 指定区域的坐标 |
| [download](./area_download.md)            | *filename* | 指定当用户单击超链接时将下载目标 |
| [href](./area_href.md)                    | *URL* | 指定区域的超链接目标 |
| [hreflang](./area_hreflang.md)            | *language\_code* | 指定目标 URL 的语言 |
| [media](./area_media.md)                  | *media query* | 指定目标 URL 优化的媒体/设备 |
| [referrerpolicy](./area_referrepolicy.md) | no-referrer <br/> no-referrer-when-downgrade <br/> origin <br/> origin-when-cross-origin <br/> same-origin <br/> strict-origin-when-cross-origin <br/> unsafe-url  | 指定与链接一起发送的推荐人信息 |
| [rel](./area_rel.md)                      | alternate <br /> author <br /> bookmark <br /> help <br /> license <br /> next <br /> nofollow <br /> noreferrer <br /> prefetch <br /> prev <br /> search <br /> tag  | 指定当前文档和目标 URL 之间的关系 |
| [shape](./area_shape.md)                  | default <br /> rect <br /> circle <br /> poly  | 指定区域的形状 |
| [target](./area_target.md)                | \_blank <br /> \_parent <br /> \_self <br /> \_top <br /> *framename* | 指定打开目标 URL 的位置 |
| [type](./area_type.md)                    | *media\_type* | 指定目标 URL 的媒体类型 |


## 全局属性

`<area>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<area>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

另一个带有可点击区域的图像地图：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126" href="a.html" alt="Sun">
  <area shape="circle" coords="90,58,3" href="address.html" alt="Mercury">
  <area shape="circle" coords="124,58,8" href="applet.html" alt="Venus">
</map>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<area>` 元素：

```css
area {
  display: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg