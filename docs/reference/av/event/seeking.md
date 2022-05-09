HTML Audio/Video DOM seeking 事件
===

## 示例

当用户开始移动/跳到视频中的新位置时，提醒一些文本：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>
<div>事件onseeking触发说明: <span id="info">....</span><div>
<script>
var vid = document.getElementById("myVideo");
vid.onseeking = function() {
  document.getElementById('info').innerHTML = '进度条操作开始';
};
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.onseeking = function() {
  document.getElementById('info').innerHTML = '进度条操作开始';
};
```

## 定义和用法

当用户开始移动/跳到音频/视频中的新位置时，会发生搜索事件。

**提示：** seek 事件与 [seeked](./seeked.md) 事件相反。

**提示：** 使用音频/视频对象的 [currentTime](../property/currenttime.md) 属性获取当前播放位置。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| seeking | Yes | 9.0 | Yes | Yes | Yes |

## 语法

在 `HTML` 中：

```html
<audio onseeking="myScript">
<video onseeking="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onseeking=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("seeking", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

### 示例

这个例子演示了 `seek` 事件和 `seeked` 事件之间的区别：

```html idoc:preview:iframe
<video onseeking="myFunction()" onseeked="mySecondFunction()" controls>
  <source src="../../../assets/horse.ogg" type="audio/ogg">
  <source src="../../../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</video>
<p>进度条开始: <span id="demo"></span> times.</p>
<p>进度条结束: <span id="demo2"></span> times.</p>
<script>
  x = 0;
  function myFunction() {
    document.getElementById("demo").innerHTML = x += 1;
  }
  y = 0;
  function mySecondFunction() {
    document.getElementById("demo2").innerHTML = y += 1;
  }
</script>
```

JavaScript:

```html
<video onseeking="myFunction()" onseeked="mySecondFunction()">
```

### 示例

当用户开始跳到新位置时，使用 Video Object 的 currentTime 属性显示当前播放时间位置：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>

<p>进度条位置: <span id="demo"></span></p>

<script>
// 获取 id="myVideo" 的 <video> 元素
var vid = document.getElementById("myVideo");
// 在 <video> 上附加一个 seeked 事件，
// 并在 seek 操作完成时执行一个函数
vid.addEventListener("seeked", myFunction);

function myFunction() {
  // 在 id="demo" 的 p 元素中显示 <video> 的当前位置
  document.getElementById("demo").innerHTML = vid.currentTime;
}
</script>
```

```js
// 获取 id="myVideo" 的 <video> 元素
var vid = document.getElementById("myVideo");
// 在 <video> 上附加一个 seeked 事件，
// 并在 seek 操作完成时执行一个函数
vid.addEventListener("seeked", myFunction);

function myFunction() {
  // 在 id="demo" 的 p 元素中显示 <video> 的当前位置
  document.getElementById("demo").innerHTML = vid.currentTime;
}
```


### 示例

当用户开始移动/跳到音频中的新位置时，提醒一些文本：

```html idoc:preview:iframe
<audio id="myAudio" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</audio>
<div>进度条操作状态: <span id="info">...</span><div>
<script>
var aud = document.getElementById("myAudio");
aud.onseeking = function() {
  document.getElementById('info').innerHTML = '进度操作完成！';
};
</script>
```

JavaScript:

```js
var aud = document.getElementById("myAudio");
aud.onseeking = function() {
  document.getElementById('info').innerHTML = '进度操作完成！';
};
```

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
