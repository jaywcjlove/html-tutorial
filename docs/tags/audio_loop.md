HTML \<audio> loop 标签
===

## 示例

一首歌曲将重新开始，每次完成时：

```html idoc:preview
<audio controls loop>
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  Your browser does not support the audio tag.
</audio>
```

## 定义和用法

`loop` 属性是一个布尔属性。

当存在时，它指定音频将在每次完成时重新开始。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| loop      | 4.0 | 9.0 | 3.5 | 4.0 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<audio loop>
```