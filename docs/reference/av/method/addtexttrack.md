HTML Audio/Video DOM addTextTrack() 方法
===

## 示例

为视频添加新的文本轨道：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">添加新的文本轨道</button><br>
<video id="video1" width="320" height="176" controls="controls">
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
var vid = document.getElementById("video1");
function myFunction() { 
  var text1 = vid.addTextTrack("caption");
  text1.addCue(new TextTrackCue("Test text", 01.000, 04.000, "", "", "", true));
} 
</script> 
```

JavaScript:

```js
var text1 = myVid.addTextTrack("caption");
text1.addCue(new TextTrackCue("Test text", 01.000, 04.000, "", "", "", true));
```

## 定义和用法

`addTextTrack()` 方法创建并返回一个新的 `TextTrack` 对象。

新的 `TextTrack` 对象被添加到音频/视频元素的文本轨道列表中。

## 浏览器支持

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| addTextTrack() | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.addTextTrack(kind,label,language)
```

## 参数值

| 值 Value | 描述 Description |
| ----- | ----- |
| *kind*     | 指定文本轨道的类型。可能的值：<br>*   `subtitles` <br>* `caption` <br>* `descriptions` <br>* `chapters` <br>*  `metadata` |
| *label*    | 一个字符串，指定文本轨道的标签。 用于为用户识别文本轨道 |
| *language* | 一个由两个字母组成的语言代码，用于指定文本轨道的语言。 要查看所有可用的语言代码，请访问我们的 [语言代码参考](../../language_codes.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

| Return Value: | 一个 TextTrack 对象，代表新的文本轨道 |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
