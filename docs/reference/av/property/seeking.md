HTML Audio/Video DOM seeking 属性
===

## 示例

显示用户当前是否正在视频中搜索：

```html idoc:preview:iframe
<video id="myVideo" controls onseeking="myFunction()" onseeked="myFunction()">
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<p>尝试在视频中寻找： <span id="mySpan"></span></p>

<script>
function myFunction() { 
  var vid = document.getElementById("myVideo");
  document.getElementById("mySpan").innerHTML = "Seeking: " + vid.seeking;
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
document.getElementById("mySpan").innerHTML = "Seeking: " + vid.seeking;
```

## 定义和用法

`seek` 属性返回用户当前是否在音频/视频 (audio/video) 中搜索。

寻找是当您移动/跳到音频/视频 (audio/video) 中的新位置时。

**注意：** 此属性是只读的。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| seeking  | Yes | 9.0 | 3.5 | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.seeking
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| Boolean | 布尔值，如果用户当前正在搜索，则返回 `true`，否则返回 `false` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
