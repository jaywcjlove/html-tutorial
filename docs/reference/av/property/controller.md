HTML Audio/Video DOM controller 属性
===

## 示例

检查视频是否有媒体控制器：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">检查视频是否有媒体控制器</button><br>
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() {
  alert("Controller: " + vid.controller);
} 
</script> 
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert("Controller: " + vid.controller);
```

## 定义和用法

控制器属性返回音频/视频的当前媒体控制器。

默认情况下，音频/视频元素没有媒体控制器。 如果指定了媒体控制器，则控制器属性会将其作为 MediaController 对象返回。

**提示：** 使用 [controls](./controls.md) 属性设置或返回视频是否应显示标准视频控件。

## 浏览器支持

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| controller | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.controller
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| MediaController Object | 表示音频/视频的媒体控制器。MediaController 对象属性/方法：<br>* `buffered` - 获取 audio/video 的缓冲范围 <br>* `seekable` - 获取 audio/video 的可搜索范围 <br>* `duration` - 获取 audio/video 的持续时间 <br>* `currentTime` - 获取或设置 audio/video 的当前播放位置 <br>* `paused` - 检查 audio/video 是否暂停 <br>* `play()` - 播放 audio/video <br>* `pause()` - 暂停 audio/video <br>* `played` - 检查 audio/video 是否已播放 <br>* `defaultPlaybackRate` - 获取或设置 audio/video 的默认播放速率 <br>* `playbackRate` - 获取或设置 audio/video 的当前播放速率 <br>* `volume` - 获取或设置 audio/video 的音量 <br>* `muted` - 获取或设置 audio/video 是否静音 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg


