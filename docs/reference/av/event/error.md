HTML Audio/Video DOM error 事件
===

在加载音频/视频期间发生错误时触发

## 示例

提示加载视频时出错：

```js
var vid = document.getElementById("myVideo");
vid.onerror = function() {
  alert("Error! Something went wrong");
};
```

## 定义和使用

在加载音频/视频期间发生错误时发生错误事件。

**提示：** 当媒体加载过程受到某种干扰时发生的相关事件是：

* [abort](./abort.md)
* emptied
* [stalled](./stalled.md)
* [suspend](./suspend.md)

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| error | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

在 `HTML` 中：

```html
<audio onerror="myScript">
<video onerror="myScript">
```

在 `JavaScript` 中：

```js
object.onerror=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
object.addEventListener("error", myScript);
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
