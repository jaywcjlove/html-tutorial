HTML \<video> 标签
===

## 示例

播放视频：

```html idoc:preview:iframe
<video width="320" controls>
  <source
    type="video/mp4"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <source
    type="video/webm"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">
  您的浏览器不支持 video 标签。
</video>
```

## 定义和用法

`<video>` 标签用于在文档中嵌入视频内容，例如电影剪辑或其他视频流。

`<video>` 标签包含一个或多个具有不同视频源的 [`<source>`](./source.md) 标签。 浏览器将选择它支持的第一个来源。

`<video>` 和 `</video>` 标签之间的文本只会在不支持 \<video> 元素的浏览器中显示。

HTML 支持三种视频格式：MP4、WebM 和 OGG。

| 浏览器 | MP4 | WebM | Ogg |
| ------- | --- | ---- | --- |
| ![edge][2]    | YES | YES  | YES |
| ![chrome][1]  | YES | YES  | YES |
| ![firefox][3] | YES | YES  | YES |
| ![safari][4]  | YES | YES  | ❌  |
| ![opera][5]   | YES | YES  | YES |

## 提示和注意事项

**提示：** 对于音频文件，请查看 [`<audio>`](./audio.md) 标签。

## Browser Support

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<video> | 4.0 | 9.0 | 3.5 | 3.1 | 11.5 |

## 可选属性

| 属性 Attribute | 值 Value | 描述 Description |
| -------- | -------- | -------- |
| [autoplay](./video_autoplay.md) | autoplay           | 指定视频一准备好就开始播放 |
| [controls](./video_controls.md) | controls           | 指定应显示视频控件（例如播放/暂停按钮等） |
| [height](./video_height.md)     | *pixels*           | 设置视频播放器的高度 |
| [loop](./video_loop.md)         | loop               | 指定视频将在每次结束时重新开始 |
| [muted](./video_muted.md)       | muted              | 指定视频的音频输出应静音 |
| [poster](./video_poster.md)     | *URL*              | 指定在视频下载时或用户点击播放按钮之前显示的图像 |
| [preload](./video_preload.md)   | auto<br>metadata<br>none | 指定当页面加载时作者是否以及如何认为应该加载视频 |
| [src](./video_src.md)           | *URL*              | 指定视频文件的 URL |
| [width](./video_width.md)       | *pixels*           | 设置视频播放器的宽度 |

## 全局属性

`<video>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<video>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 相关页面

HTML Audio/Video DOM 参考: [HTML Audio/Video DOM Reference](../reference/av_dom.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg