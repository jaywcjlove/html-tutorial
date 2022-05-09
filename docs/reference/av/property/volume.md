HTML Audio/Video DOM volume 属性
===

## 示例

将视频音量设置为 20%：

```html idoc:preview:iframe
<button onclick="getVolume()" type="button">音量是多少？</button>
<button onclick="setHalfVolume()" type="button">将音量设置为 0.2</button>
<button onclick="setFullVolume()" type="button">将音量设置为 1.0</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
  var vid = document.getElementById("myVideo");
  function getVolume() { 
    alert(vid.volume);
  }
  function setHalfVolume() { 
    vid.volume = 0.2;
  }
  function setFullVolume() { 
    vid.volume = 1.0;
  }
</script>
```

```js
var vid = document.getElementById("myVideo");
vid.volume = 0.2;
```

## 定义和用法

`volume` 属性设置或返回音频/视频 (audio/video) 的当前音量。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| volume   | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回音量属性：

```js
audio|video.volume
```

设置音量属性：

```js
audio|video.volume=number
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | 指定音频/视频(audio/video)的当前音量。 必须是介于 0.0 和 1.0 之间的数字。 示例值：<br>* 1.0 是最高音量（100%。这是默认值） <br>* 0.5 是一半体积 (50%) <br>* 0.0 为静音（与静音相同） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值:  | 一个数字，表示当前音量 |
| 返回值: | `1.0` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

