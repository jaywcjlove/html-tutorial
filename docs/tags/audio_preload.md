HTML \<audio> preload 标签
===

## 示例

作者认为页面加载时不应该加载声音：

```html idoc:preview
<audio controls preload="none">
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
```

## 定义和用法

`preload` 属性指定作者是否以及如何认为在页面加载时应该加载音频文件。

`preload` 属性允许作者向浏览器提供关于他/她认为会带来最佳用户体验的提示。 在某些情况下，此属性可能会被忽略。

**注意：** 如果存在 `autoplay`，则忽略 preload 属性。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| preload   | 4.0 | 9.0 | 4.0 | 4.0 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<audio preload="auto|metadata|none">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| auto     | 作者认为页面加载时浏览器应该加载整个音频文件 |
| metadata | 作者认为页面加载时浏览器应该只加载元数据 |
| none     | 作者认为页面加载时浏览器不应该加载音频文件 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg