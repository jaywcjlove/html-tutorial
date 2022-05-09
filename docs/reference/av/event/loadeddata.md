HTML Audio/Video DOM loadeddata 事件
===

## 示例

提醒当前帧的数据可用（对于 \<video>）：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持音频元素。
</video>
<div>加载状态:<span id="info">正在加载中...</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.onloadeddata = function() {
  document.getElementById('info').innerHTML = '浏览器已加载当前帧';
};
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.onloadeddata = function() {
  document.getElementById('info').innerHTML = '浏览器已加载当前帧';
};
```

## 定义和用法

当加载当前帧的数据，但没有足够的数据播放指定音频/视频的下一帧时，会发生 `loadeddata` 事件。

在音频/视频的加载过程中，会依次发生以下事件：

1.  [loadstart](./loadstart.md)
2.  [durationchange](./durationchange.md)
3.  [loadedmetadata](./loadedmetadata.md)
4.  loadeddata
5.  [progress](./progress.md)
6.  [canplay](./canplay.md)
7.  [canplaythrough](./canplaythrough.md)

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| loadeddata | Yes | 9.0 | Yes | Yes | Yes |

## Syntax

在 `HTML` 中：

```html
<audio onloadeddata="myScript">
<video onloadeddata="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onloadeddata=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("loadeddata", myScript);
```

## Technical Details

| 支持的 HTML 标签: | \<audio> and \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

提醒当前帧的数据可用（对于 \<audio>）：

```html idoc:preview:iframe
<audio id="myAudio" controls>
  <source src="../../../assets/horse.ogg" type="audio/ogg">
  <source src="../../../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>
<div>加载状态:<span id="info">正在加载中...</span><div>
<script>
var aud = document.getElementById("myAudio");
aud.onloadeddata = function() {
  document.getElementById('info').innerHTML = '浏览器已加载当前帧';
};
</script> 
```

JavaScript:

```js
var aud = document.getElementById("myAudio");
aud.onloadeddata = function() {
  document.getElementById('info').innerHTML = '浏览器已加载当前帧';
};
```



[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
