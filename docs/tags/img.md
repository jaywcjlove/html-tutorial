HTML \<img> Tag
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

**提示：** 要将图像链接到另一个文档，只需将 `<img>` 标记嵌套在 [<a>](./a.md) 标记内（参见下面的示例）。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<img>  | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [alt](att_img_alt.asp) | *text* | Specifies an alternate text for an image |
| crossorigin | anonymous use-credentials | Allow images from third-party sites that allow cross-origin access to be used with canvas                                |
| [height](att_img_height.asp)                | *pixels*                                                                          | Specifies the height of an image                                                                                         |
| [ismap](att_img_ismap.asp)                  | ismap                                                                             | Specifies an image as a server-side image map                                                                            |
| [loading](att_img_loading.asp)              | eager lazy                                                                        | Specifies whether a browser should load an image immediately or to defer loading of images until some conditions are met |
| [longdesc](att_img_longdesc.asp)            | *URL*                                                                             | Specifies a URL to a detailed description of an image                                                                    |
| [referrerpolicy](att_img_referrepolicy.asp) | no-referrer no-referrer-when-downgrade origin origin-when-cross-origin unsafe-url | Specifies which referrer information to use when fetching an image                                                       |
| sizes                                       | *sizes*                                                                           | Specifies image sizes for different page layouts                                                                         |
| [src](att_img_src.asp)                      | *URL*                                                                             | Specifies the path to the image                                                                                          |
| srcset                                      | *URL-list*                                                                        | Specifies a list of image files to use in different situations                                                           |
| [usemap](att_img_usemap.asp)                | *#mapname*                                                                        | Specifies an image as a client-side image map                                                                            |
| [width](att_img_width.asp)                  | *pixels*                                                                          | Specifies the width of an image                                                                                          |

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