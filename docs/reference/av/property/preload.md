HTML Audio/Video DOM preload 属性
===

## 示例

页面加载后立即开始加载视频：

```html idoc:preview:iframe
<button onclick="enablePreload()" type="button">启用预加载</button>
<button onclick="disablePreload()" type="button">禁用预加载</button>
<button onclick="checkPreload()" type="button">检查预加载状态</button><br>

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
  var vid = document.getElementById("myVideo");
  function enablePreload() { 
    vid.preload = "auto";
  }
  function disablePreload() { 
    vid.preload = "none";
  }
  function checkPreload() { 
    alert(vid.preload);
  }
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.preload = "auto";
```

## 定义和用法

`preload` 属性设置或返回是否应在页面加载后立即开始加载音频/视频(audio/video)。

`preload` 属性允许作者向浏览器提供最佳用户体验的提示。 在某些情况下，此属性可能会被忽略。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| preload  | Yes | 9.0 | 4.0 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回预加载属性：

```js
audio|video.preload
```

设置预加载属性：

```js
audio|video.preload="auto|metadata|none"
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| auto     | 指示音频/视频(audio/video)应在页面加载后立即开始加载 |
| metadata | 指示在页面加载时仅应加载音频/视频(audio/video)的元数据 |
| none     | 指示音频/视频(audio/video)不应在页面加载后立即开始加载 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个字符串，表示应预加载哪些数据（如果有）。 可能的返回值为 `auto`、 `metadata`或 `none`。 有关这些值的含义，请参阅 [属性值](#属性值) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg


