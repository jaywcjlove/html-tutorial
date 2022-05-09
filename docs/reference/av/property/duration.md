HTML Audio/Video DOM duration 属性
===

## 示例

获取当前视频的长度：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取视频长度</button><br>
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.duration);
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("video1");
alert(vid.duration);
```

## 定义和用法

duration 属性返回当前音频/视频(audio/video)的长度，以秒为单位。

如果没有设置音频/视频(audio/video)，则返回 NaN (Not-a-Number)。

**注意：** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| duration | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.duration
```

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个数字，表示视频的长度，以秒为单位。 如果未设置视频，则返回 `NaN`（非数字）。 如果视频是流式传输的并且没有预定义的长度，则返回 `Inf`（无穷大）。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
