HTML Audio/Video DOM ratechange 事件
===

## 示例

更改视频的播放速度并提醒速度已更改：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" autoplay controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>
<br>
<div>触发事件展示说明: <span id="info">....</span><div>
<button onclick="setPlaySpeed()" type="button">将视频设置为慢动作播放</button>

<script>
  // 获取 id="myVideo" 的 <video> 元素
  var vid = document.getElementById("myVideo");
  // 将视频的当前播放速度设置为 0.3（慢动作）
  function setPlaySpeed() {
    vid.playbackRate = 0.3;
  }
  // 为 <video> 元素分配一个 ratechange 事件，
  // 如果视频的播放速度发生变化，则执行一个函数。 该功能将提醒一些文本
  vid.onratechange = function() {myFunction()};

  function myFunction() {
    document.getElementById('info').innerHTML = 'ondatechange 事件发生 - 视频的播放速度发生了变化';
  }
</script>
```

JavaScript:

```js
// 获取 id="myVideo" 的 <video> 元素
var vid = document.getElementById("myVideo");

// 将视频的当前播放速度设置为 0.3（慢动作）
function setPlaySpeed() {
  vid.playbackRate = 0.3;
}

// 为 <video> 元素分配一个 ratechange 事件，
// 如果视频的播放速度发生变化，则执行一个函数。 该功能将提醒一些文本
vid.onratechange = function() {myFunction()};
function myFunction() {
  document.getElementById('info').innerHTML = 'ondatechange 事件发生 - 视频的播放速度发生了变化';
}
```

## 定义和使用

`ratechange` 事件在音频/视频的播放速度发生变化时发生（例如当用户切换到慢动作或快进模式时）。

此事件由音频/视频对象的 [playbackRate](./playbackrate.md) 属性调用，该属性设置或返回音频/视频的当前播放速度。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| ratechange | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onratechange="myScript">
<video onratechange="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onratechange=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("ratechange", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

