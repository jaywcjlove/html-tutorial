HTML Audio/Video DOM currentSrc 属性
===

## 示例

获取当前视频地址：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取当前视频地址</button><br>
 
<video id="myVideo" controls="controls">
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.currentSrc);
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.currentSrc);
```


## 定义和用法

`currentSrc` 属性返回当前 audio/video 的 URL。

如果没有设置 audio/video，则返回一个空字符串。

**注意：** 此属性是只读的。

**提示：** 使用 [src](./src.md) 属性设置视频文件的 URL。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| currentSrc | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.currentSrc
```

## 技术细节

|   |   |
| ----- | ----- |
| 返回值: | 一个 String，代表当前音视频的URL。 返回整个 URL，包括协议（如 `http://`）。 如果没有设置音频/视频(audio/video)，则返回一个空字符串 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

