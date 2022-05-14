HTML \<img> 标签
===

## 示例

如何插入图像：

```html idoc:preview
<img src="../assets/editors-001.png" alt="Girl in a jacket" height="300">
```
<!--rehype:style=min-height: 300px;-->

## 定义和用法

`<img>` 标签用于在 HTML 页面中嵌入图像。

从技术上讲，图像不会插入网页； 图像链接到网页。 `<img>` 标签为引用的图像创建一个保存空间。

`<img>` 标签有两个必需的属性：

* src - 指定图像的路径
* alt - 如果由于某种原因无法显示图像，则为图像指定替代文本

**注意：** 此外，请始终指定图像的宽度和高度。 如果未指定宽度和高度，则在加载图像时页面可能会闪烁。

**提示：** 要将图像链接到另一个文档，只需将 `<img>` 标签嵌套在 [<a>](./a.md) 标签内（参见下面的示例）。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<img>  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [alt](./img_alt.md) | *text* | 指定图像的替代文本|
| crossorigin | anonymous<br>use-credentials | 允许使用允许跨域访问的第三方站点的图像canvas                                |
| [height](./img_height.md)                | *pixels* | 指定图像的高度|
| [ismap](./img_ismap.md)                  | ismap | 将图像指定为服务器端图像映射|
| [loading](./img_loading.md)              | eager <br> lazy | 指定浏览器应该立即加载图像还是推迟加载图像直到满足某些条件|
| [longdesc](./img_longdesc.md)            | *URL* | 指定图像详细描述的 URL|
| [referrerpolicy](./img_referrepolicy.md) | no-referrer<br>no-referrer-when-downgrade<br>origin<br>origin-when-cross-origin<br>unsafe-url | 指定在获取图像时要使用的引荐来源信息|
| sizes                                       | *sizes* | 指定不同页面布局的图像大小|
| [src](./img_src.md)                      | *URL* | 指定图像的路径|
| srcset                                      | *URL-list* | 指定在不同情况下使用的图像文件列表|
| [usemap](./img_usemap.md)                | *#mapname* | 将图像指定为客户端图像映射|
| [width](./img_width.md)                  | *pixels* | 指定图像的宽度|
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<img>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<img>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

Align image (with CSS):

```html idoc:preview
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="vertical-align:bottom">
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="vertical-align:middle">
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="vertical-align:top">
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="float:right">
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="float:left">
```

添加图像边框（使用 CSS）：

```html idoc:preview
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="border:5px solid black">
```

为图像添加左右边距（使用 CSS）：

```html idoc:preview
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="vertical-align:middle;margin:0px 50px">
```

为图像添加顶部和底部边距（使用 CSS）：

```html idoc:preview
<img src="../assets/chrome.svg" alt="Smiley face" width="42" height="42" style="vertical-align:middle;margin:50px 0px">
```
<!--rehype:style=min-height: 120px;-->

如何从另一个文件夹或另一个网站插入图像：

```html idoc:preview
<img src="../assets/chrome.svg" alt="Stickman" width="24" height="39">
<img src="../assets/sublime_text.png" alt="Lamp" width="32" height="32">
```

如何为图片添加超链接：

```html idoc:preview
<a href="https://github.com/jaywcjlove/html-tutorial">
  <img src="../assets/sublime_text.png" alt="HTML Tutorial" width="100" height="132">
</a>
```
<!--rehype:style=min-height: 132px;-->

如何创建带有可点击区域的图像地图。 每个区域都是一个超链接：

```html idoc:preview
<img src="../assets/sublime_text.png" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="iframe" href="iframe.html">
  <area shape="rect" coords="290,172,333,250" alt="footer" href="footer.htm">
  <area shape="circle" coords="337,300,44" alt="embed Tag" href="embed.htm">
</map>
```

## 相关页面

HTML 教程: [HTML Images](../tutorial/images.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<img>` 元素：

```css
img {
  display: inline-block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg