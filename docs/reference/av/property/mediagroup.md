HTML Audio/Video DOM mediaGroup 属性
===

## 示例

为 2 个视频设置媒体组：

```html idoc:preview:iframe
<button onclick="setMedGroup()" type="button">为视频设置媒体组</button>
<button onclick="getMedGroup()" type="button">获取视频的媒体组</button><br> 

<video id="myVideo1" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<video id="myVideo2" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
  var vid1 = document.getElementById("myVideo1");
  var vid2 = document.getElementById("myVideo2");
  function setMedGroup() { 
    vid1.mediaGroup="test";
    vid2.mediaGroup="test";
  }
  function getMedGroup() { 
    alert("视频 1 媒体组: " + vid1.mediaGroup +
    ". 视频 2 媒体组: " + vid2.mediaGroup);
  } 
</script> 
```

JavaScript:

```js
var vid1 = document.getElementById("myVideo1");
var vid2 = document.getElementById("myVideo2");
vid1.mediaGroup = "test";
vid2.mediaGroup = "test";
```

## 定义和用法

`mediaGroup` 属性设置或返回音频/视频(audio/video)所属的媒体组的名称。

一个媒体组允许 2 个或更多音频/视频(audio/video)元素保持同步。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| `mediaGroup` | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回 `mediaGroup` 属性：

```js
audio|video.mediaGroup
```

设置 `mediaGroup` 属性：

```js
audio|video.mediaGroup="group"
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *group* | 指定音频/视频(audio/video)的媒体组 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个字符串。 指示音频/视频(audio/video)的媒体组 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg


