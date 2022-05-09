HTML Audio/Video DOM waiting 事件
===

## 示例

提醒视频需要缓冲下一帧才能开始播放：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>
<div>事件 onwaiting 触发: <span id="info">....</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.onwaiting = function() {
  document.getElementById('info').innerHTML = '等待！ 我需要缓冲下一帧';
};
</script>
```

```js
var vid = document.getElementById("myVideo");
vid.onwaiting = function() {
  document.getElementById('info').innerHTML = '等待！ 我需要缓冲下一帧';
};
```

## 定义和使用

等待事件发生在视频停止时，因为它需要缓冲下一帧。

此事件也可用于 \<audio> 元素，但主要用于视频。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| waiting | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onwaiting="myScript">
<video onwaiting="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onwaiting=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("waiting", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

