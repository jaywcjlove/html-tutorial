HTML Audio/Video DOM currentTime 属性
===

## 示例

将时间位置设置为 5 秒：

```html idoc:preview:iframe
<button onclick="getCurTime()" type="button">获取当前时间位置</button>
<button onclick="setCurTime()" type="button">将时间位置设置为 5 秒</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function getCurTime() { 
  alert(vid.currentTime);
}
function setCurTime() { 
  vid.currentTime=5;
}
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.currentTime = 5;
```

## 定义和用法

`currentTime` 属性设置或返回音频/视频(audio/video)播放的当前位置（以秒为单位）。

设置该属性时，播放会跳转到指定位置。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| currentTime | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回 `currentTime` 属性：

```js
audio|video.currentTime
```

设置 `currentTime` 属性：

```js
audio|video.currentTime="seconds"
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *seconds* | 指示音频/视频(audio/video)播放的位置，以秒为单位 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个数字，以秒为单位表示当前播放时间 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
