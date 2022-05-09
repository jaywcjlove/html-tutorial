HTML Audio/Video DOM ended 属性
===

## 示例

检查视频播放是否结束：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">视频播放结束了吗？</button><br>
 
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");

function myFunction() { 
  alert(vid.ended);
} 
</script> 
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.ended);
```


## 定义和用法

`ended` 属性返回音频/视频(audio/video)的播放是否已经结束。

当播放位置在音频/视频(audio/video)的末尾时，音频/视频已结束。

**注意⚠️:** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| ended    | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.ended
```

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个布尔值，如果播放结束返回true，否则返回false |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

