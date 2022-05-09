HTML Audio/Video DOM play 事件
===

## 示例

提醒视频已开始播放：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>
<div>加载状态: <span id="info">可以播放了</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.onpause = function() {
  document.getElementById('info').innerHTML = '视频已暂停';
};
vid.onplay = function() {
  document.getElementById('info').innerHTML = '视频已开始播放';
};
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.onplay = function() {
  document.getElementById('info').innerHTML = '视频已开始播放';
};
```

## 定义和用法

播放事件发生在音频/视频已开始或不再暂停时。

**提示：** [pause](./pause.md) 事件在音频/视频暂停时发生。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| play  | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onplay="myScript">
<video onplay="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onplay=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("play", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> and \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

提示音频已开始播放：

```html idoc:preview:iframe
<audio id="myAudio" controls>
  <source src="../../../assets/horse.ogg" type="audio/ogg">
  <source src="../../../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>
<div>加载状态: <span id="info">可以播放了</span><div>
<script>
var aud = document.getElementById("myAudio");
aud.onplay = function() {
  document.getElementById('info').innerHTML = '音频已开始播放';
};
</script>
```

```js
var aud = document.getElementById("myAudio");
aud.onplay = function() {
  document.getElementById('info').innerHTML = '音频已开始播放';
};
```


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
