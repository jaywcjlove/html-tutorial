HTML Audio/Video DOM error 属性
===

## 示例

获取视频的错误状态：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">获取错误状态</button><br>
<video id="myVideo" width="320" height="176" controls autoplay>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>
<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.error.code);
} 
</script>
```

**注意：** 此属性仅在 Internet Explorer 9 和更新版本中受支持。

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.error.code);
```

## 定义和用法

`error` 属性返回一个 `MediaError` 对象。

`MediaError` 对象有一个 code 属性，其中包含音频/视频(audio/video)的错误状态。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| error    | ❌ 不支持 | 9.0  | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.error.code
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| Number | MediaError 对象的 code 属性返回一个数字，表示音频/视频的错误状态：<br>* 1 = `MEDIA_ERR_ABORTED` - 获取过程被用户中止 <br>* 2 = `MEDIA_ERR_NETWORK` - 下载时出错 <br>* 3 = `MEDIA_ERR_DECODE` - 解码时出错 <br>* 4 = `MEDIA_ERR_SRC_NOT_SUPPORTED` - 不支持音频/视频 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
