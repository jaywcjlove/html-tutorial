HTML Audio/Video DOM play() 方法
===

## 示例

带有播放(play)和暂停(pause)按钮的视频：

```html idoc:preview:iframe
<button onclick="playVid()" type="button">Play Video</button>
<button onclick="pauseVid()" type="button">Pause Video</button><br>
<video id="myVideo" width="320" height="176">
  <source id="mp4_src" src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script> 
var vid = document.getElementById("myVideo"); 
function playVid() { 
  vid.play(); 
}
function pauseVid() { 
  vid.pause(); 
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
function playVid() {
  vid.play();
}
function pauseVid() {
  vid.pause();
}
```

## 定义和用法

`play()` 方法开始播放当前的 [\<audio>](../../../tags/audio.md) / [\<video>](../../../tags/video.md)。

**提示：** 使用 [pause()](av_met_pause.md) 方法暂停当前的 [\<audio>](../../../tags/audio.md) / [\<video>](../../../tags/video.md)。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| play() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.play()
```

## 参数

|      |
| ---- |
| None |
<!--rehype:style=width: 100%; display: inline-table;-->

## 返回值

|                 |
| ---- |
| 无返回值 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
