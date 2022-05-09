HTML Audio/Video DOM load() 方法
===

## 示例

更改视频源并重新加载视频：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">更换视频</button><br>
<video id="myVideo" controls autoplay>
  <source id="mp4_src" src="../../../assets/mov_bbb11.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script> 
function myFunction() { 
  document.getElementById("mp4_src").src = "../../../assets/mov_bbb.mp4";
  document.getElementById("myVideo").load();
} 
</script> 
```

JavaScript:

```js
document.getElementById("mp4_src").src = "movie.mp4";
document.getElementById("myVideo").load();
```

## 定义和用法

`load()` 方法重新加载 [\<audio>](../../../tags/audio.md)/[\<video>](../../../tags/video.md) 元素。

`load()` 方法用于在更改源或其他设置后更新 [\<audio>](../../../tags/audio.md)/[\<video>](../../../tags/video.md) 元素。

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| load() | Yes | 9.0 | Yes | 6.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.load()
```

## 参数

|      |
| ---- |
| None |
<!--rehype:style=width: 100%; display: inline-table;-->

## 返回值

|                 |
| ---- |
| 无返回值 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
