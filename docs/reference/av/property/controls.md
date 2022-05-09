HTML Audio/Video DOM controls 属性
===

## 示例

启用视频控件：

```html idoc:preview:iframe
<button onclick="enableControls()" type="button">启用控件</button>
<button onclick="disableControls()" type="button">禁用控件</button>
<button onclick="checkControls()" type="button">检查控件状态</button><br>
<video id="myVideo" width="320" height="176">
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
  var vid = document.getElementById("myVideo");
  function enableControls() { 
    vid.controls = true;
    vid.load();
  }
  function disableControls() { 
    vid.controls = false;
    vid.load();
  }
  function checkControls() { 
    alert(vid.controls);
  }
</script> 
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
function enableControls() { 
  vid.controls = true;
  vid.load();
}
function disableControls() { 
  vid.controls = false;
  vid.load();
}
function checkControls() { 
  alert(vid.controls);
}
```

## 定义和用法

`controls` 属性设置或返回浏览器是否应显示标准 audio/video 控件。

标准 audio/video 控制应包括：

* Play 播放
* Pause 暂停
* Seeking 进度条
* Volume 音量
* 全屏切换（供视频）
* Captions/Subtitles 字幕（当可用时）
* Track 轨道（当可用时）

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| controls | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回控件属性：

```js
audio|video.controls
```

设置控件属性：

```js
audio|video.controls=true|false
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| `true`  | 表示显示控件 |
| `false` | 默认。 表示不显示控件 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

| 返回值:  | 布尔值，如果显示控件则返回 true，否则返回 false |
| ----- | ----- |
| 默认值: | `false` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
