HTML Audio/Video DOM 中止事件
===

## 定义和用法

警告视频的加载已中止：

```js
var vid = document.getElementById("myVideo");
vid.onabort = function() {
  alert("Video load aborted");
};
```

## 定义和用法

`abort` 事件在音频/视频的加载被中止时发生。

此事件在媒体数据下载被中止时发生，而不是因为错误。

**提示：** 当媒体加载过程受到某种干扰时发生的相关事件是：

*   emptied
*   [error](../events/onerror.md)
*   [stalled](../events/onstalled.md)
*   [suspend](av_event_suspend.asp)

## 浏览器支持

表中的数字指定了完全支持该事件的第一个浏览器版本。

| Event | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| abort | Yes | 9.0 | Yes | Yes | Yes |

**注意：** Windows 7 上的 Internet Explorer 11 不支持中止事件。

## 语法

在 HTML 中:

```html
<element onabort="myScript">
```

在 `JavaScript` 中:

```js
object.onabort = function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
object.addEventListener("abort", myScript);
```

## 技术细节

| 支持的 HTML 标签：          | [\<audio>](../tags/audio.md) 和 [\<video>](../tags/video.md) |
| ----------------------------- | --------------------- |
| 支持的 JavaScript 对象： | Audio, Video          |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg