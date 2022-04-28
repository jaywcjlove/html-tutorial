HTML \<audio> Tag
===

## 示例

播放声音文件：

```html idoc:preview
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio tag.
</audio>
```

## 定义和用法

`<audio>` 标签用于在文档中嵌入声音内容，例如音乐或其他音频流。

`<audio>` 标签包含一个或多个具有不同音频源的 `<source>` 标签。 浏览器将选择它支持的第一个来源。

`<audio>` 和 `</audio>` 标签之间的文本只会在不支持 `<audio>` 元素的浏览器中显示。

HTML 支持三种音频格式：MP3、WAV 和 OGG。

### 音频格式和浏览器支持

| Browser   | MP3 | WAV   | OGG   |
| --------- | --- | ----- | ----- |
| Edge / IE | YES | YES\* | YES\* |
| Chrome    | YES | YES   | YES   |
| Firefox   | YES | YES   | YES   |
| Safari    | YES | YES   | ❌    |
| Opera     | YES | YES   | YES   |

## 提示和注意事项

**提示：** 对于视频文件，请查看 [`<video>`](./video.md) 标签。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | ---- |
| \<audio> | 4.0 | 9.0 | 3.5 | 4.0 | 11.5 |

## 属性

| Attribute | Value | Description |
| ------- | ------- | ------- |
| [autoplay](./audio_autoplay.md) | autoplay           | 指定音频一准备好就开始播放 |
| [controls](./audio_controls.md) | controls           | 指定应显示音频控件（例如播放/暂停按钮等） |
| [loop](./audio_loop.md)         | loop               | 指定音频将在每次结束时重新开始 |
| [muted](./audio_muted.md)       | muted              | 指定音频输出应静音 |
| [preload](./audio_preload.md)   | auto metadata none | 指定当页面加载时作者是否以及如何认为应该加载音频 |
| [src](./audio_src.md)           | *URL*              | 指定音频文件的 URL |


## 全局属性

`<audio>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<audio>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg