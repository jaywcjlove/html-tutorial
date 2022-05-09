HTML Audio/Video DOM defaultMuted 属性
===

## 示例

将视频设置为默认静音：

```html idoc:preview:iframe
<button onclick="getMuted()" type="button">视频是否默认静音？</button>
<button onclick="setToMuted()" type="button">将视频设置为默认静音，并重新加载视频</button><br>
 
<video id="myVideo" width="320" height="176" controls>
  <source src="../../../assets/mov_bbb.mp4" type="video/mp4">
  您的浏览器不支持 HTML5 视频。
</video>

<script>
var vid = document.getElementById("myVideo");
function getMuted() { 
  alert(vid.defaultMuted);
}
function setToMuted() { 
  vid.defaultMuted = true;
  vid.load()
}
</script>
```

JavaScript:

```js
var vid = document.getElementById("myVideo");
vid.defaultMuted = true;
```

## 定义和用法

`defaultMuted` 属性设置或返回音频/视频(audio/video)是否应默认静音。

设置此属性只会更改默认静音状态，而不是当前状态。 要更改当前静音状态，请使用 [muted](./muted.md) 属性。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Property | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| defaultMuted | Yes | ❌ 不支持 | 11.0 | 6.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

返回 defaultMuted 属性：

```js
audio|video.defaultMuted
```

设置 defaultMuted 属性：

```js
audio|video.defaultMuted=true|false
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| `true`  | 表示音频/视频(audio/video)默认静音 |
| `false` | 默认。 表示音频/视频(audio/video)默认不静音 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|  |  |
| ----- | ----- |
| 返回值:  | 一个布尔值，如果音频/视频默认静音，则返回 `true`，否则返回 `false` |
| 默认值: | `false` |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

