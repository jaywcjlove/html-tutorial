HTML muted 属性
===

## 定义和用法

`muted` 属性是一个布尔属性。

当存在时，它指定视频的音频输出应该被静音。

## 适用于

`muted` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<video>](../tags/video.md) | [muted](../tags/video_muted.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

静音视频：

```html idoc:preview:iframe
<video width="320" controls muted>
  <source
    type="video/mp4"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <source
    type="video/webm"
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">
  您的浏览器不支持 video 标签。
</video>
```



## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| muted     | 4.0 | 10.0 | 11.0 | 7.1 | 10.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg