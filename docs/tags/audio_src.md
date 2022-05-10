HTML \<audio> src 标签
===

## 示例

播放声音：

```html idoc:preview
<audio controls src="../assets/horse.mp3">
  您的浏览器不支持音频标签。
</audio>
```

## 定义和用法

`src` 属性指定音频文件的位置（URL）。

上面的示例使用 Ogg 文件，并且可以在 Firefox、Opera、Chrome 和 Edge 中运行。 但是，要在 IE 或 Safari 中播放音频文件，我们必须使用 MP3 文件。

要使其在所有浏览器中工作 - 在 `<audio>` 元素中使用 [\<source>](tag_source.asp) 元素。 每个 `<source>` 元素可以链接到不同的音频文件。 浏览器将使用第一个识别的格式：

## 示例

```html idoc:preview
<audio controls preload="none">
  <source src="../assets/horse.ogg" type="audio/ogg">
  <source src="../assets/horse.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| src       | 4.0 | 9.0 | 3.5 | 4.0 | 11.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** `src` 属性在所有主流浏览器中均受支持，但文件格式可能并非在所有浏览器中均受支持！

## 语法

```html
<audio src="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 音频文件的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `src="http://www.example.com/horse.ogg"`） <br>* 相对 URL - 指向网站内的文件（如 `src="horse.ogg"`） |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg