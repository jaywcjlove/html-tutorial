HTML height 属性
===

## 示例

`height` 属性指定元素的高度，以像素为单位。

## 适用于

`height` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<canvas>](../tags/canvas.md) | [height](../tags/canvas_height.md) |
| [\<embed>](../tags/embed.md)   | [height](../tags/embed_height.md)  |
| [\<iframe>](../tags/iframe.md) | [height](../tags/iframe_height.md) |
| [\<img>](../tags/img.md)       | [height](../tags/img_height.md)    |
| [\<input>](../tags/input.md)   | [height](../tags/input_height.md)  |
| [\<object>](../tags/object.md) | [height](../tags/object_height.md) |
| [\<video>](../tags/video.md)   | [height](../tags/video_height.md)  |

## 示例

### Canvas 示例

一个高度和宽度为 200 像素的 [\<canvas>](../tags/canvas.md) 元素：

```html idoc:preview:iframe
<canvas id="myCanvas" width="200" height="200" style="border:1px solid">
```
<!--rehype:style=height: 200px;-->

### Embed 示例

一个高度和宽度为 200 像素的 Flash 动画：

```html idoc:preview:iframe
<embed src="helloworld.swf" width="200" height="200">
```
<!--rehype:style=height: 200px;-->

### Iframe 示例

指定高度和宽度为 200 像素的 [\<iframe>](../tags/iframe.md)：

```html idoc:preview:iframe
<iframe src="./header.html" width="200" height="200">
</iframe>
```
<!--rehype:style=height: 200px;-->

### Img 示例

一个高度和宽度为 42 像素的图像：

```html idoc:preview:iframe
<img src="../assets/chrome.svg" alt="Smiley face" height="42" width="42">
```

### Input 示例

定义一个图像作为提交按钮，具有高度和宽度属性：

```html idoc:preview:iframe
<form action="/action_page.php">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="image" src="../assets/chrome.svg" alt="Submit" width="48" height="48">
</form>
```

### Object 示例

一个高度和宽度为 400 像素的 Flash 动画:

```html
<object data="helloworld.swf" height="400" width="400"></object>
```

### Video 示例

具有指定高度和宽度的视频播放器：

```html idoc:preview:iframe
<video width="320" controls>
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

`height` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [\<canvas>](../tags/canvas.md) | 4.0 | 9.0 | 2.0  | 3.1 | 9.0 |
| [\<embed>](../tags/embed.md)   | Yes | Yes | Yes  | Yes | Yes |
| [\<iframe>](../tags/iframe.md) | Yes | Yes | Yes  | Yes | Yes |
| [\<img>](../tags/img.md)       | Yes | Yes | Yes  | Yes | Yes |
| [\<input>](../tags/input.md)   | 1.0 | Yes | 16.0 | Yes | 1.0 |
| [\<object>](../tags/object.md) | Yes | Yes | Yes  | Yes | Yes |
| [\<video>](../tags/video.md)   | Yes | Yes | Yes  | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
