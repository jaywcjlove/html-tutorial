HTML \<embed> 标签
===

## 示例

嵌入图像：

```html idoc:preview
<embed type="image/jpg" src="../assets/editors-006.png" width="300" height="160">
```
<!--rehype:style=min-height: 200px;-->

嵌入的 HTML 页面：

```html idoc:preview
<embed type="text/html" src="./dt.html" width="500" height="200">
```
<!--rehype:style=min-height: 200px;-->

嵌入视频：

```html idoc:preview
<embed type="video/webm" src="video.mp4" width="400" height="300">
```
<!--rehype:style=min-height: 200px;-->

## 定义和用法

`<embed>` 标签定义了外部资源的容器，例如网页、图片、媒体播放器或插件应用程序。

## 警告 ⚠️

大多数浏览器不再支持 Java 小程序和插件。

任何浏览器都不再支持 ActiveX 控件。

现代浏览器也关闭了对 Shockwave Flash 的支持。

## 建议

要显示图片，最好使用 [`<img>`](./img.md) 标签。

要显示 HTML，最好使用 [`<iframe>`](./iframe.md) 标签。

要显示视频或音频，最好使用 [`<video>`](./video.md) 和 [`<audio>`](./audio.md) 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<embed> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| [height](./embed_height.md) | *pixels*      | 指定嵌入内容的高度 |
| [src](./embed_src.md)       | *URL*         | 指定要嵌入的外部文件的地址 |
| [type](./embed_type.md)     | *media\_type* | 指定嵌入内容的媒体类型 |
| [width](./embed_width.md)   | *pixels*      | 指定嵌入内容的宽度 |

## 全局属性

`<embed>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<embed>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<embed>` 元素：

```css
embed:focus {
  outline: none;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg