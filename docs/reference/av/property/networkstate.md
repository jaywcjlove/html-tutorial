HTML Audio/Video DOM networkState 属性
===

## 示例

获取视频的当前网络状态：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取网络状态</button><br> 

<video id="myVideo" width="320" height="176" controls autoplay>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.networkState);
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.networkState);
```

## 定义和用法

`networkState` 属性返回音频/视频(audio/video)的当前网络状态（activity）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| networkState | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.networkState
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| Number | 表示音频/视频(audio/video)元素的当前网络状态：<br>* 0 = `NETWORK_EMPTY` - 音频/视频(audio/video)尚未初始化 <br>* 1 = `NETWORK_IDLE` - 音频/视频(audio/video)处于活动状态并已选择资源，但未使用网络 <br>* 2 = `NETWORK_LOADING` - 浏览器正在下载数据 <br>* 3 = `NETWORK_NO_SOURCE` - 未找到音频/视频(audio/video)源 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

