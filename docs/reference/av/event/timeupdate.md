HTML Audio/Video DOM timeupdate 事件
===

## 示例

当视频的播放位置发生变化时，以秒为单位显示视频的当前位置：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video>

<p>播放位置： <span id="demo"></span></p>

<script>
// 获取 id="myVideo" 的视频元素
var vid = document.getElementById("myVideo");

// 为视频元素分配一个ontimeupdate事件，
// 如果当前播放位置发生变化则执行一个函数
vid.ontimeupdate = function() {myFunction()};

function myFunction() {
  // 在 id="demo" 的 p 元素中显示视频的当前位置
  document.getElementById("demo").innerHTML = vid.currentTime;
}
</script>
```

JavaScript:

```js
// 获取 id="myVideo" 的视频元素
var vid = document.getElementById("myVideo");

// 为视频元素分配一个ontimeupdate事件，
// 如果当前播放位置发生变化则执行一个函数
vid.ontimeupdate = function() {myFunction()};

function myFunction() {
  // 在 id="demo" 的 p 元素中显示视频的当前位置
  document.getElementById("demo").innerHTML = vid.currentTime;
}
```

## 定义和使用

`timeupdate` 事件在音频/视频的播放位置发生变化时发生。

此事件由以下方式调用：

*播放音频/视频
* 移动播放位置（比如当用户快进到音频/视频中的不同点时）

**提示：**这个timeupdate事件常与音频/视频对象的[currentTime](./currenttime.md)属性一起使用，它返回音频/视频播放的当前位置，以秒为单位。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| timeupdate | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio ontimeupdate="myScript">
<video ontimeupdate="myScript">
```

在 `JavaScript` 中：

```js
audio|video.ontimeupdate=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("timeupdate", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

### 示例

当音频的播放位置发生变化时，以秒为单位显示音频的当前位置：

```html idoc:preview:iframe
<audio id="myAudio" controls>
  <source src="../../../assets/horse.ogg" type="audio/ogg">
  <source src="../../../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频元素。
</audio>

<p>播放位置: <span id="demo"></span></p>
<script>
// 获取 id="myAudio" 的 <audio> 元素
var aud = document.getElementById("myAudio");

// 将 ontimeupdate 事件分配给 <audio> 元素，
// 如果当前播放位置发生变化，则执行一个函数
aud.ontimeupdate = function() {myFunction()};
function myFunction() {
  // 在 id="demo" 的 <p> 元素中显示音频的当前位置
  document.getElementById("demo").innerHTML = aud.currentTime;
}
</script>
```

```js
// 获取 id="myAudio" 的 <audio> 元素
var aud = document.getElementById("myAudio");

// 将 ontimeupdate 事件分配给 <audio> 元素，
// 如果当前播放位置发生变化，则执行一个函数
aud.ontimeupdate = function() {myFunction()};

function myFunction() {
  // 在 id="demo" 的 <p> 元素中显示音频的当前位置
  document.getElementById("demo").innerHTML = aud.currentTime;
}
```

### 示例

使用 currentTime 属性将当前播放位置设置为 5 秒：

```html idoc:preview:iframe
<video id="myVideo" width="320" height="240" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  <source src="../../../assets/mov_bbb.ogg" type="video/ogg">
  您的浏览器不支持 HTML5 视频。
</video><br>

<button onclick="setCurTime()" type="button">将时间位置设置为 5 秒</button>
<p id="demo"></p>

<script>
// 获取 id="myVideo" 的视频元素
var vid = document.getElementById("myVideo");

// 将“timeupdate”事件附加到视频
vid.addEventListener("timeupdate", getCurTime);

// 在 id="demo" 的 p 元素中显示视频的当前播放位置
function getCurTime() { 
  document.getElementById("demo").innerHTML = "当前播放位置是 " + vid.currentTime + " 秒。";
} 

// 将当前播放位置设置为 5 秒
function setCurTime() { 
  vid.currentTime = 5;
} 
</script>
```

```js
document.getElementById("myVideo").currentTime = 5;
```


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
