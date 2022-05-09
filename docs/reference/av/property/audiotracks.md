HTML Audio/Video DOM audioTracks 属性
===

## 示例

获取可用音轨的数量：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取可用音轨的数量</button>
<br>
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.audioTracks.length);
} 
</script> 
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.audioTracks.length);
```

## 定义和用法

`audioTracks` 属性返回一个 `AudioTrackList` 对象。

`AudioTrackList` 对象表示音频/视频的可用音轨。

每个可用的音轨都由一个 `AudioTrack` 对象表示。

## 浏览器支持

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| audioTracks | ❌ 不支持 | 11 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |

## 语法

```js
audio|video.audioTracks
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| AudioTrackList Object | 表示 audio/video.AudioTrackList 对象的可用音轨：<br>* audioTracks.length - 获取可用音轨的数量 <br>* audioTracks.getTrackById(*id*) - 通过 id 获取 AudioTrack 对象 <br>* audioTracks\[*index*] - 通过索引获取 AudioTrack 对象<br>**注意：** 第一个可用的 AudioTrack 对象是 *index* 0 |
| AudioTrack Object     | 表示一个音轨。AudioTrack 对象属性：<br>* `id` - 获取音轨的 id <br>* `kind` - 获取音轨的类型（可以是：`alternative`、`description`、`main`、`translation`、`commentary` 或 `空字符串`） <br>* `label` - 获取音轨的标签 <br>* `language` - 获取音轨的语言 <br>* `enabled` - 如果轨道处于活动状态，则获取或设置 (true/false) |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

