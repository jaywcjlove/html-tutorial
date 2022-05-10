HTML \<audio> autoplay 属性
===

## 示例

将自动开始播放的音频文件：

```html idoc:preview
<audio controls autoplay>
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
```

## 定义和用法

`autoplay` 属性是一个布尔属性。

当存在时，音频将立即自动开始播放而不会停止。

**注意：** Chromium 浏览器在大多数情况下不允许自动播放。 但是，始终允许静音自动播放。

在 `autoplay` 之后添加 `muted` 让您的音频文件开始自动播放（但静音）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| autoplay  | 4.0 | 9.0 | 3.5 | 4.0 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<audio autoplay>
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg