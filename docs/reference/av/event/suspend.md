HTML Audio/Video DOM suspend 事件
===

## 示例

警告媒体数据的加载被阻止继续：

```js
var vid = document.getElementById("myVideo");
vid.onsuspend = function() {
  alert("Loading of the media is suspended");
};
```

## 定义和使用

当浏览器故意不获取媒体数据时，会发生挂起事件。

此事件在媒体加载暂停（阻止继续）时发生。 这可能在下载完成时发生，或者由于某种原因已暂停。

**提示：** 当媒体加载过程受到某种干扰时发生的相关事件是：

* [abort](./abort.md)
* emptied
* [error](./error.md)
* [stalled](./stalled.md)

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| suspend | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onsuspend="myScript">
<video onsuspend="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onsuspend=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("suspend", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->




[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg
