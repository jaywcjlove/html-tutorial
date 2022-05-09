HTML Audio/Video DOM readyState 属性
===

## 示例

获取视频的当前就绪状态：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">准备就绪状态</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.readyState);
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.readyState);
```

## 定义和用法

`readyState` 属性返回音频/视频 (audio/video) 的当前就绪状态。

就绪状态指示音频/视频 (audio/video) 是否准备好播放。

**注意：** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| readyState | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.readyState
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| Number | 表示音频/视频元素的就绪状态：<br>* 0 = `HAVE_NOTHING` - 没有关于音频/视频是否就绪的信息 <br>* 1 = `HAVE_METADATA` - 音频/视频的元数据已准备就绪 <br>* 2 = `HAVE_CURRENT_DATA` - 当前播放位置的数据可用，但没有足够的数据播放下一帧/毫秒 <br>* 3 = `HAVE_FUTURE_DATA` - 当前和至少下一帧的数据可用 <br>* 4 = `HAVE_ENOUGH_DATA` - 有足够的可用数据开始播放 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg



