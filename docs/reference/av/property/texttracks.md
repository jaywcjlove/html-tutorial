HTML Audio/Video DOM textTracks 属性
===

## 示例

获取可用文本轨道的数量：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取可用文本轨道的数量</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <track src="../../../assets/demo_sub.vtt">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
  var vid = document.getElementById("myVideo");
  function myFunction() { 
    alert(vid.textTracks.length);
  }
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.textTracks.length);
```

## 定义和用法

`textTracks` 属性返回一个 `TextTrackList` 对象。

`TextTrackList` 对象表示音频/视频的可用文本轨道。

每个可用的文本轨道都由一个 `TextTrack` 对象表示。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| textTracks | Yes | 10.0 | 33.0 | 6.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.textTracks
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| TextTrackList Object | 表示音频/视频的可用文本轨道。TextioTrackList 对象：<br>* 长度 - 获取音频/视频中可用的文本轨道数 <br>* \[*index*] - 通过索引获取 TextTrack 对象<br>**注意：** 第一个可用的 TextTrack 对象是 *index* 0 |
| TextTrack Object     | 表示一个文本轨道。TextTrack 对象属性：<br>* kind - 获取文本轨道的类型（可以是：`subtitles`、`caption`、`descriptions`、`chapters`或`metadata`） <br>* label - 获取文本轨道的标签 <br>* language - 获取文本轨道的语言 <br>* mode - 获取或设置轨道是否处于活动状态（`disabled`,`hidden`,`showing`） <br>* cues - 获取 cue 列表作为 TextTrackCueList 对象 <br>* activeCues - 获取当前活动的文本轨道提示作为 TextTrackCueList 对象 <br>* addCue(*cue*) - 在提示列表中添加一个提示 <br>* removeCue(*cue*) - 从提示列表中删除一个提示 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

