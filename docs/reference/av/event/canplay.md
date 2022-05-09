HTML Audio/Video DOM canplay 事件
===

## 示例

提醒视频已准备好开始播放：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">您的浏览器不支持 HTML5 视频。
</video>
<div>加载状态:<span id="info">正在加载中...</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.oncanplay = function() {
  document.getElementById('info').innerHTML = '可以开始播放视频了';
};
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.oncanplay = function() {
    alert("可以开始播放视频了");
};
```

## 定义和用法

当浏览器可以开始播放指定的音频/视频 (audio/video)（当它缓冲到足以开始播放时）时，会发生 canplay 事件。

在音频/视频 (audio/video)的加载过程中，会依次发生以下事件：

1. [loadstart](./loadstart.md)
2. [durationchange](./durationchange.md)
3. [loadedmetadata](./loadedmetadata.md)
4. [loadeddata](./loadeddata.md)
5. [progress](./progress.md)
6. canplay
7. [canplaythrough](./canplaythrough.md)

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| canplay | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio oncanplay="myScript">
<video oncanplay="myScript">
```

在 `JavaScript` 中：

```js
audio|video.oncanplay = function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("canplay", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

提示音频已准备好开始播放：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">您的浏览器不支持 HTML5 视频。
</video>
<div>加载状态:<span id="info">正在加载中...</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.oncanplay = function() {
  document.getElementById('info').innerHTML = '可以开始播放视频了';
};
</script>
```

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
