HTML Audio/Video DOM src 属性
===

## 示例

更改视频来源：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">更换视频</button><br>
<video id="myVideo" controls autoplay>
  <source src="../../../assets/mov_bbb1111.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script> 
var vid = document.getElementById("myVideo");
function myFunction() { 
  isSupp = vid.canPlayType("video/mp4");
  if (isSupp == "") {
    vid.src = "../../../assets/mov_bbb.ogg";
  } else {
    vid.src = "../../../assets/mov_bbb.mp4";
  }
  vid.load();
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.src = "movie.ogg";
```

## 定义和用法

`src` 属性设置或返回音频/视频 (audio/video) 的当前源。

源是音频/视频 (audio/video) 文件的实际位置 (URL)。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| src      | Yes | 9.0 | 3.5 | Yes | Yes |

## 语法

返回 src 属性：

```js
audio|video.src
```

设置 src 属性：

```js
audio|video.src=URL
```

## 返回值

| 类型 Type | 描述 Description |
| -------- | -------- |
| *URL* | 指定音频/视频源的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `src="http://www.example.com/movie.ogg"`） <br>* 相对 URL - 指向网站内的文件（如 `src="movie.ogg"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个String，代表音视频文件的URL。 返回整个 URL，包括协议（如 `http://`） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

获取 video 视频的来源（URL）：

```html idoc:preview:iframe
<video id="myVideo" width="320" controls src="../../../assets/mov_bbb.mp4">您的浏览器不支持 HTML5 视频。 </video>

<div>单击按钮以获取视频的 URL。</div>
<button onclick="myFunction()">尝试一下</button>
<div id="demo"></div>

<script>
function myFunction() {
  var vid = document.getElementById("myVideo").src;
  document.getElementById("demo").innerHTML = vid;
}
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo").src;
```

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

