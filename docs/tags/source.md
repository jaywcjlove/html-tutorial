HTML \<source> Tag
===

## 示例

带有两个源文件的音频播放器。 浏览器会选择第一个

```html idoc:preview:iframe
<audio controls>
  <source src="../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持音频元素。
</audio>
```

## 定义和用法

`<source>` 标签用于为媒体元素指定多个媒体资源，例如 [\<video>](./video.md)、[\<audio>](./audio.md) 和 [\<picture>](./picture.md)。

`<source>` 标签允许您指定浏览器可以选择的替代视频/音频/图像文件，基于浏览器支持或视口宽度。 浏览器会选择它支持的第一个 `<source>`。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<source> | 4.0 | 9.0 | 3.5 | 4.0 | 10.5 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [media](./source_media.md)   | *media\_query* | 接受通常在 CSS 中定义的任何有效媒体查询 |
| sizes                        |                | 指定不同页面布局的图像大小 |
| [src](./source_src.md)       | *URL*          | 在 [\<audio>](./audio.md) 和 [\<video>](./video.md) 中使用 \<source> 时需要。 指定媒体文件的 URL |
| [srcset](./source_srcset.md) | *URL*          | 在 [\<picture>](./picture.md) 中使用 \<source> 时是必需的。 指定要在不同情况下使用的图像的 URL |
| [type](./source_type.md)     | *MIME-type*    | 指定资源的 MIME 类型 |

## 全局属性

`<source>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<source>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

在 [\<video>](./video.md) 中使用 \<source> 播放视频：

```html idoc:preview:iframe
<video width="320" controls>
  <source src="../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

在 \<picture> 中使用 \<source> 根据视口宽度定义不同的图像：

```html idoc:preview:iframe
<picture>
  <source srcset="../assets/example.png" media="(max-width: 600px)">
  <source srcset="../assets/sublime_text.png" media="(max-width: 1500px)">
  <source srcset="../assets/chrome.svg">
  <img src="../assets/example.png" alt="Flowers" style="width:auto;">
</picture>
```
<!--rehype:style=height: 290px;-->

## 相关页面

HTML 教程: [HTML Video](../tutorial/video.md)

HTML 教程: [HTML Audio](../tutorial/audio.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg