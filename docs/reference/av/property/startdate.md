HTML Audio/Video DOM startDate 属性
===

## 示例

获取视频的当前时间轴偏移量：

```html idoc:preview:iframe
<button onclick="myFunction()" type="button">Get timeline offset</button><br> 

<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function myFunction() { 
  alert(vid.startDate);
} 
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
alert(vid.startDate);
```

## 定义和用法

`startDate` 属性返回一个 `Date` 对象，表示音频/视频的当前时间轴偏移量。

`startDate` 属性用于启用通过 `Internet` 实时流式传输的音频/视频的准确同步。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| startDate | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```js
audio|video.startDate
```

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个日期对象，表示当前时间线偏移 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

