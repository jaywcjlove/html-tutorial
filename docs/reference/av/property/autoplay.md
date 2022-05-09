HTML Audio/Video DOM autoplay 属性
===

## 示例

启用自动播放并重新加载视频：

```html idoc:preview:iframe
<button onclick="enableAutoplay()" type="button">启用自动播放</button>
<button onclick="disableAutoplay()" type="button">禁用自动播放</button>
<button onclick="checkAutoplay()" type="button">检查自动播放状态</button><br><br>
<video id="myVideo" width="320" height="176" controls="controls">
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
  var vid = document.getElementById("myVideo");
  function enableAutoplay() { 
    vid.autoplay = true;
    vid.load();
  }
  function disableAutoplay() { 
    vid.autoplay = false;
    vid.load();
  }
  function checkAutoplay() { 
    alert(vid.autoplay);
  }
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.autoplay = true;
vid.load();
```

## 定义和用法

`autoplay` 属性设置或返回音频/视频是否应在加载后立即开始播放。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| autoplay | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回自动播放属性：

```js
audio|video.autoplay
```

设置自动播放属性：

```js
audio|video.autoplay=true|false
```

## 参数值

| 值 Value | 描述 Description |
| ----- | ----- |
| `true`  | 指示音频/视频应在加载后立即开始播放 |
| `false` | 默认。 指示音频/视频不应在加载后立即开始播放 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

| 返回值:  | 一个布尔值。 无论真假 |
| ----- | ----- |
| 默认值: | `false` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg


