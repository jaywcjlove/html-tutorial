HTML loop 属性
===

[![](https://shields.io/badge/HTML5-<audio>兼容-green?logo=HTML5)](https://caniuse.com/mdn-html_elements_audio_loop)
[![](https://shields.io/badge/HTML5-<video>兼容-green?logo=HTML5)](https://caniuse.com/mdn-html_elements_video_loop)

## 定义和用法

`loop` 属性是一个布尔属性。

当存在时，它指定音频将在每次完成时重新开始。

## 适用于

`loop` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<audio>](../tags/audio.md) | [loop](../tags/audio_loop.md) |
| [\<video>](../tags/video.md) | [loop](../tags/video_loop.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Audio 示例

一首歌曲将重新开始，每次完成时：

```html idoc:preview:iframe
<audio controls loop>
  <source type="audio/ogg" src="horse.ogg">
  <source type="audio/mpeg" src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3">
  您的浏览器不支持音频元素。
</audio>
```

### Video 示例

每次完成后都会重新开始的视频：

```html idoc:preview:iframe
<video width="320" controls loop>
  <source
    type="video/mp4"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <source
    type="video/webm"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">
    您的浏览器不支持 video 标签。
</video>
```

## 浏览器支持

`loop` 属性对每个元素都有以下浏览器支持：

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<audio>](../tags/audio.md) loop | 4.0 | 9.0 | 3.5  | 4.0 | 10.5 |
| [\<video>](../tags/video.md) loop | 4.0 | 9.0 | 11.0 | 4.0 | 10.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg