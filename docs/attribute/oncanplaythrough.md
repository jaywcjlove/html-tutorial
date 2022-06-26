HTML oncanplaythrough  属性
===

## 定义和用法

`oncanplaythrough` 事件发生在浏览器估计它可以播放指定的 audio/video 而无需停止缓冲时。

## 适用于

`oncanplaythrough` 属性是 [事件属性](../reference/eventattributes.md) 的一部分，可用于以下元素：

| 元素 | 事件 |
| --- | --- |
| [\<audio>](../tags/audio.md) | [canplaythrough](../reference/av/event/canplaythrough.md) |
| [\<video>](../tags/video.md) | [canplaythrough](../reference/av/event/canplaythrough.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Audio 示例

当音频准备好开始播放时运行 `myFunction`：

```html
<audio oncanplaythrough="myFunction()">
```


```html idoc:preview:iframe
<script>
  function myFunction() {
    alert("可以开始播放音频");
  }
</script> 
<audio controls oncanplaythrough="myFunction()">
  <source type="audio/ogg" src="horse.ogg">
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
```


### Video 示例

当视频准备好开始播放时运行 `myFunction`：

```html
<video oncanplaythrough="myFunction()">
```

```html idoc:preview:iframe
<script>
  function myFunction() {
    alert("可以开始播放视频了");
  }
</script> 
<video width="320" controls oncanplaythrough="myFunction()">
  <source type="video/mp4" src="../assets/mov_bbb.mp4">
  <source type="video/ogm" src="../assets/mov_bbb.ogm">
  您的浏览器不支持 video 标签。
</video>
```

## 浏览器支持

`oncanplaythrough` 属性对每个元素都有以下浏览器支持：

| 元素 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| audio   | Yes | 9.0 | Yes | Yes | Yes |
| video   | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
