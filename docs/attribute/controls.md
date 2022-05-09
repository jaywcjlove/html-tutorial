HTML controls 属性
===

## 定义和用法

`controls` 属性是一个布尔属性。

如果存在，它指定应显示音频/视频控件。

控制应包括：

* 播放 Play
* 暂停 Pause
* Seeking
* 音量 Volume
* 全屏切换（仅适用于 video 视频）
* 字幕/字幕 (仅适用于 video 视频，如果可用)
* 轨道 (仅适用于 video 视频，如果可用)

## 适用于

`controls` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<audio>](../tags/audio.md) | [controls](../tags/audio_controls.md) |
| [\<video>](../tags/video.md) | [controls](../tags/video_controls.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Audio 示例

带有浏览器默认控件的 [\<audio>](../tags/audio.md) 元素：

```html idoc:preview:iframe
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>
```

### Video 示例

带有浏览器默认控件的 [\<video>](../tags/video.md) 元素：

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

## 浏览器支持

`controls` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [audio](../tags/audio.md)   | 4.0 | 9.0 | 3.5 | 4.0 | 10.5 |
| [video](../tags/video.md)   | 4.0 | 9.0 | 3.5 | 4.0 | 10.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg