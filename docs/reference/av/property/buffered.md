HTML Audio/Video DOM buffered 属性
===

## 示例

以秒为单位获取视频的第一个缓冲范围（部分）：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取第一个缓冲范围</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">您的浏览器不支持 HTML5 视频。
</video>
<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert("Start: " + vid.buffered.start(0) + " End: "  + vid.buffered.end(0));
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert("Start: " + vid.buffered.start(0)
+ " End: " + vid.buffered.end(0));
```

## 定义和用法

`buffered` 属性返回一个 `TimeRanges` 对象。

`TimeRanges` 对象表示用户缓冲的 audio/video 范围。

缓冲范围是缓冲 audio/video 的时间范围。 如果他跳过 audio/video，用户将获得几个缓冲范围。

**注意：** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| buffered | Yes | 9.0 | 4.0  | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.buffered
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| TimeRanges Object | 表示音频/视频的缓冲部分。TimeRanges 对象属性：<br>* `length` - 获取音频/视频中缓冲范围的数量 <br>* `start(index)` - 获取缓冲范围的起始位置 <br>* `end(index)` - 获取缓冲范围的结束位置<br>**注意：** 第一个缓冲范围是 *index* 0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

