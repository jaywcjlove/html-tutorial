HTML autoplay 属性
===

## 定义和用法

`autoplay` 属性是一个布尔属性。

当存在时，音频/视频将立即自动开始播放而不会停止。

## 适用于

`autoplay` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<audio>](../tags/audio.md) | [autoplay](../tags/audio_autoplay.md) |
| [\<video>](../tags/video.md) | [autoplay](../tags/video_autoplay.md) |

## 示例

将自动开始播放的音频文件：

```html idoc:preview:iframe
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>
```

将自动开始播放的视频：

```html idoc:preview:iframe
<video width="320" autoplay>
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

`autoplay` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [audio](../tags/audio.md)   | 4.0 | 9.0 | 3.5 | 4.0 | 10.5 |
| [video](../tags/video.md)   | 4.0 | 9.0 | 3.5 | 4.0 | 10.5 |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg