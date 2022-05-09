HTML Audio/Video DOM videoTracks 属性
===

## 示例

获取可用视频轨道的数量：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取可用视频轨道的数量</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.videoTracks.length);
} 
</script>
```

```js
var vid = document.getElementById("myVideo");
alert(vid.videoTracks.length);
```

## 定义和用法

`videoTracks` 属性返回一个 `VideoTrackList` 对象。

`VideoTrackList` 对象表示视频的可用视频轨道。

每个可用的视频轨道都由一个 `VideoTrack` 对象表示。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| videoTracks | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
video.videoTracks
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| VideoTrackList Object | 表示 video.VideoTrackList 对象的可用视频轨道： <br>* videoTracks.length - 获取视频中可用的视频轨道数 <br>* videoTracks.getTrackById(*id*) - 通过 id 获取 VideoTrack 对象 <br>* videoTracks\[*index*] - 通过索引获取 VideoTrack 对象 <br>* videoTracks.selectedIndex - 获取当前VideoTrack对象的索引<br>**注意：** 第一个可用的VideoTrack对象是*index* 0 |
| VideoTrack Object     | 表示一个视频轨道。VideoTrack对象属性：<br>* id - 获取视频轨道的id <br>* kind - 获取视频轨道的类型（可以是：`alternative`、`captions`、`main`、`sign`、`subtitles`、`commentary`或 `空字符串`） <br>* label - 获取视频轨道的标签 <br>* language - 获取视频轨道的语言 <br>* selected - 如果轨道处于活动状态，则获取或设置 (true\|false) |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

