HTML Audio/Video DOM seekable 属性
===

## 示例

以秒为单位获取视频的第一个可搜索范围（部分）：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取第一个可搜索范围</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert("Start: " + vid.seekable.start(0) + " End: "  + vid.seekable.end(0));
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert("Start: " + vid.seekable.start(0) + " End: " + vid.seekable.end(0));
```

## 定义和用法

`seekable` 属性返回一个 `TimeRanges` 对象。

`TimeRanges` 对象表示可供用户搜索的音频/视频 (audio/video) 范围。

可搜索范围是用户可以搜索（移动播放位置）到的音频/视频 (audio/video) 的时间范围。

对于非流媒体视频，即使在缓冲之前，通常也可以在视频中的任何位置寻找。

**注意：** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| seekable | Yes | 9.0 | 8.0 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.seekable
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| TimeRanges Object | 表示音频/视频的可搜索部分。TimeRanges 对象属性：<br>* length - 获取音频/视频中可搜索范围的数量 <br>* start(*index*) - 获取可搜索范围的起始位置 <br>* end(*index*) - 获取可搜索范围的结束位置<br>**注意：** 第一个可搜索范围是 *index* 0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
