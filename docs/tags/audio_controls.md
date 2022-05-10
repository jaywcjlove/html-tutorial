HTML \<audio> controls 标签
===

## 示例

带有浏览器默认控件的 \<audio> 元素：

```html idoc:preview
<audio controls>
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
```

## 定义和用法

`controls` 属性是一个布尔属性。

如果存在，它指定应显示音频控件。

音频控制应包括：

*   Play 播放
*   Pause 暂停
*   Seeking 进度条
*   Volume 音量


## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| controls  | 4.0 | 9.0 | 3.5 | 4.0 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<audio controls>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg