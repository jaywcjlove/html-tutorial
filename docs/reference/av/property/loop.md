HTML Audio/Video DOM loop 属性
===

## 示例

将视频设置为循环播放：

```html idoc:preview:iframe
<button onclick="enableLoop()" type="button">启用循环</button>
<button onclick="disableLoop()" type="button">禁用循环</button>
<button onclick="checkLoop()" type="button">检查循环状态</button><br><br>

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function enableLoop() { 
  vid.loop = true;
  vid.load();
}
function disableLoop() { 
  vid.loop = false;
  vid.load();
}
function checkLoop() { 
  alert(vid.loop);
}
</script>
```

```js
var vid = document.getElementById("myVideo");
vid.loop = true;
```

## 定义和用法

`loop` 属性设置或返回音频/视频(audio/video)完成后是否应该重新开始播放。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| loop     | Yes | 9.0 | 11.0 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回循环属性：

```js
audio|video.loop
```

设置循环属性：

```js
audio|video.loop=true|false
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| `true`  | 表示音频/视频结束后应重新开始播放 |
| `false` | 默认。 表示音频/视频结束后不应再次开始播放 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值:  | 一个布尔值，如果音频/视频重新开始播放，则在每次播放结束时返回 `true`。 否则返回 `false` |
| 默认值: | `false` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg


