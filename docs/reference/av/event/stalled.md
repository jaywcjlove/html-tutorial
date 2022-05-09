HTML Audio/Video DOM stalled 事件
===

## 示例

如果浏览器无法获取媒体数据，请提醒媒体数据不可用：

```js
var vid = document.getElementById("myVideo");
vid.onstalled = function() {
  alert("媒体数据不可用");
};
```

## 定义和使用

当浏览器尝试获取媒体数据但数据不可用时，会发生停滞事件。

**提示：** 当媒体加载过程受到某种干扰时发生的相关事件是：

* [abort](./abort.md)
* emptied
* [error](./error.md)
* [suspend](./suspend.md)

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 事件 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| stalled | Yes | 9.0 | Yes | Yes | Yes |

## 语法

在 `HTML` 中：

```html
<audio onstalled="myScript">
<video onstalled="myScript">
```

在 `JavaScript` 中：

```js
audio|video.onstalled=function(){ myScript };
```

在 `JavaScript` 中，使用 `addEventListener()` 方法：

```js
audio|video.addEventListener("stalled", myScript);
```

## 技术细节

| 支持的 HTML 标签: | \<audio> 和 \<video> |
| -------- | -------- |
| 支持的 JavaScript 对象: | Audio, Video |
<!--rehype:style=width: 100%; display: inline-table;-->
