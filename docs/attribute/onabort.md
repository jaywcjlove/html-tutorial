HTML onabort 属性
===

## 定义和用法

`onabort` 属性定义了在媒体文件加载中止时要运行的脚本。

此事件在媒体数据下载被中止时发生，而不是因为错误。

## 适用于

`onabort` 属性是 [Event Attributes](../reference/eventattributes.md) 的一部分，可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<audio>](../tags/audio.md)   | [onabort](../events/onabort.md) |
| [\<embed>](../tags/embed.md)   | onabort                       |
| [\<img>](../tags/img.md)       | onabort                       |
| [\<object>](../tags/object.md) | onabort                       |
| [\<video>](../tags/video.md)   | [onabort](../events/onabort.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

警告视频的加载已中止：

```html
<video id="myVideo" onabort="alert('Video load aborted')">
```

## 浏览器支持

`onabort` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<audio>](../tags/audio.md)   | Yes | 9.0           | Yes | Yes | Yes |
| [\<embed>](../tags/embed.md)   | Yes | ❌ 不支持 | Yes | Yes | Yes |
| [\<img>](../tags/img.md)       | Yes | Yes           | Yes | Yes | Yes |
| [\<object>](../tags/object.md) | Yes | ❌ 不支持 | Yes | Yes | Yes |
| [\<video>](../tags/video.md)   | Yes | 9.0           | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** Windows 7 上的 Internet Explorer 11 不支持音频/视频的中止事件。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg