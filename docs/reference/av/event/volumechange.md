HTML Audio/Video DOM volumechange 事件
===

## 示例

提醒视频的音量已更改：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>
<div>事件 onvolumechange 触发: <span id="info">....</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.onvolumechange = function() {
  document.getElementById('info').innerHTML = '音量已更改';
};
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.onvolumechange = function() {
  document.getElementById('info').innerHTML = '音量已更改';
};
```

## 定义和使用

每次更改视频/音频的音量时都会发生 volumechange 事件。

此事件由以下方式调用：

* 增加或减少音量
* 静音或取消静音媒体播放器

**提示：** 使用音频/视频对象的 [volume](./volume.md) 属性设置或返回音频/视频的音量。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| volumechange | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onvolumechange="myScript">
<video onvolumechange="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onvolumechange=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("volumechange", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

警告音频文件的音量已更改：

```html idoc:preview:iframe
<audio id="myAudio" controls>
  <source src="../../../assets/horse.ogg" type="audio/ogg">
  <source src="../../../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>
<div>音量已更触发: <span id="info">....</span><div>
<script>
var aud = document.getElementById("myAudio");
aud.onvolumechange = function() {
  document.getElementById('info').innerHTML = '音量已更改';
};
</script>
```

JavaScript:

```js
var aud = document.getElementById("myAudio");
aud.onvolumechange = function() {
  document.getElementById('info').innerHTML = '音量已更改';
};
```


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
