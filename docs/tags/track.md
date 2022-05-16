HTML \<track> 标签
===

## 示例

带有两种语言的字幕轨道的视频：

```html idoc:preview:iframe
<video width="320" controls>
  <source
    type="video/mp4"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <source
    type="video/webm"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">
  <track src="fgsubtitles_en.vtt" kind="subtitles" srclang="en" label="English">
  <track src="fgsubtitles_no.vtt" kind="subtitles" srclang="no" label="Norwegian">
</video>
```

## 定义和用法

`<track>` 标签为 [\<audio>](./audio.md) 或 [\<video>](./video.md) 元素指定文本轨道。

此元素用于指定字幕、字幕文件或其他包含文本的文件，这些文件在媒体播放时应该可见。

曲目采用 WebVTT 格式（.vtt 文件）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<track> | 23.0 | 10.0 | 31.0 | 6.0 | 12.1 |

## 可选属性

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [default](./track_default.md) | default                                           | 指定如果用户的偏好没有表明另一个轨道更合适，则启用该轨道 |
| [kind](./track_kind.md)       | captions chapters descriptions metadata subtitles | 指定文本轨道的类型 |
| [label](./track_label.md)     | *text*                                            | 指定文本轨道的标题 |
| [src](./track_src.md)         | *URL*                                             | 必需的。 指定轨道文件的 URL |
| [srclang](./track_srclang.md) | *language\_code*                                  | 指定轨道文本数据的语言（如果 kind="subtitles" 是必需的） |

## 全局属性

`<track>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<track>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Video](../tutorial/video.md)

HTML 教程: [HTML Audio](../tutorial/audio.md)

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg