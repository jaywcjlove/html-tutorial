HTML Audio/Video DOM defaultPlaybackRate 属性
===

## 示例

默认将视频设置为慢动作：

```html idoc:preview:iframe
<button onclick="getPlaySpeed()" type="button">默认播放速度是多少？</button>
<button onclick="setPlaySpeed()" type="button">将视频设置为慢动作播放</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");

function getPlaySpeed() { 
  alert(vid.defaultPlaybackRate);
} 

function setPlaySpeed() { 
  vid.defaultPlaybackRate = 0.5;
  vid.load();
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.defaultPlaybackRate = 0.5;
```

## 定义和用法

`defaultPlaybackRate` 属性设置或返回音频/视频(audio/video)的默认播放速度。

设置此属性只会更改默认播放速度，而不是当前播放速度。 要更改当前播放速度，请使用 [playbackRate](./playbackrate.md) 属性。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| `defaultPlaybackRate` | Yes | 9.0 | 20.0 | ❌ 不支持 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回 `defaultPlaybackRate` 属性：

```js
audio|video.defaultPlaybackRate
```

设置 `defaultPlaybackRate` 属性：

```js
audio|video.defaultPlaybackRate=playbackspeed
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *playbackspeed* | 指示音频/视频的默认播放速度。 示例值：<br>* `1.0` 是正常速度 <br>* `0.5` 是半速（较慢） <br>* `2.0` 为双倍速度（更快） <br>* `-1.0` 是向后，正常速度 <br>* `-0.5` 是向后，半速 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值:  | 数字，默认播放速度 |
| 默认值: | `1.0` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

