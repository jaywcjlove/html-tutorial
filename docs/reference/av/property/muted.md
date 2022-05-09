HTML Audio/Video DOM muted 属性
===

## 示例

关闭视频的声音：

```html idoc:preview:iframe
<button onclick="enableMute()" type="button">静音</button>
<button onclick="disableMute()" type="button">启用声音</button>
<button onclick="checkMute()" type="button">检查静音状态</button><br><br>

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
  var vid = document.getElementById("myVideo");
  function enableMute() { 
    vid.muted = true;
  }
  function disableMute() { 
    vid.muted = false;
  }
  function checkMute() { 
    alert(vid.muted);
  }
</script>
```

JavaScript:

```js
var vid = document.getElementById("video1");
vid.muted = true;
```

## 定义和用法

`muted` 属性设置或返回音频/视频(audio/video)是否应该静音（声音关闭）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| muted    | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回 `muted` 属性：

```js
audio|video.muted
```

设置 `muted` 属性：

```js
audio|video.muted=true|false
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| `true`  | 表示应关闭音频/视频的声音 |
| `false` | 默认。 表示应该为音频/视频打开声音 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值:  | 布尔值，如果声音关闭则返回 `true`，否则返回 `false` |
| 默认值: | `false` |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

