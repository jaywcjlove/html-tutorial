HTML \<audio> muted 标签
===

## 示例

静音音频：

```html idoc:preview
<audio controls muted>
  <source type="audio/ogg" src="horse.ogg">
  <source type="audio/mpeg" src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3">
  您的浏览器不支持音频标签。
</audio>
```

## 定义和用法

`muted` 属性是一个布尔属性。

当存在时，它指定音频输出应该被静音。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| muted     | 4.0 | 10.0 | 11.0 | 7.1 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<audio muted>
```