HTML default 属性
===

## 定义和用法

`default` 属性是一个布尔属性。

当存在时，它指定如果用户的偏好没有指示另一个轨道会更合适，则启用该轨道。

**注意：** 每个 `<media>` 元素不能有多个具有 `default` 属性的 [`<track>`](../tags/track.md) 元素。

## 适用于

`default` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<track>](../tags/track.md) | [default](../tags/track_default.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

带有两个字幕轨道的视频。 “英文”字幕是默认的：

```html
<video width="320" height="240" controls>
  <source src="forrest_gump.mp4" type="video/mp4">
  <source src="forrest_gump.ogg" type="video/ogg">
  <track src="subtitles_en.vtt" kind="subtitles" srclang="en" label="English" default>
  <track src="subtitles_no.vtt" kind="subtitles" srclang="no" label="Norwegian">
</video>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| default   | 18.0 | 10.0 | 31.0 | 6.0 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg