HTML Audio/Video DOM canPlayType() 方法
===

## 示例

检查您的浏览器是否可以播放不同类型的视频：

```html idoc:preview:iframe
<p>我的浏览器可以播放 MP4 视频吗？ <span>
<button onclick="supportType(event,'video/mp4','avc1.42E01E, mp4a.40.2')" type="button">Test</button>
</span></p>

<p>我的浏览器可以播放 OGG 视频吗？<span>
<button onclick="supportType(event,'video/ogg','theora, vorbis')" type="button">Test</button>
</span></p>
<script> 
function supportType(e,vidType,codType) { 
  var vid = document.createElement('video');
  isSupp = vid.canPlayType(vidType+';codecs="'+codType+'"');
  if (isSupp == "") { isSupp = "No"; }
  e.target.parentNode.innerHTML = "答案: " + isSupp;
} 
</script> 
```

JavaScript:

```js
var vid = document.createElement('video');
isSupp = vid.canPlayType(vidType+';codecs="'+codType+'"');
```

## 定义和用法

`canPlayType()` 方法检查浏览器是否可以播放指定的音频/视频类型。

`canPlayType()` 方法可以返回以下值之一：

* `probably` - 浏览器最有可能支持这种音频/视频类型
* `maybe` - 浏览器可能支持这种音频/视频类型
* "" - （空字符串）浏览器不支持这种音频/视频类型

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| -------- | --- | --- | --- | --- | --- |
| `canPlayType()` | Yes | 9.0 | Yes | Yes | Yes |

## 语法

```js
audio|video.canPlayType(type)
```

## 参数值

| 值 | 描述 Description |
| ----- | ----- |
| *type* | 指定要测试支持的音频/视频类型（和可选编解码器）。 共同值：<br>* video/ogg <br>* video/mp4 <br>* video/webm <br>* audio/mpeg <br>* audio/ogg <br>* audio/mp4<br>常用值，包括编解码器：<br>*   video/ogg; codecs="theora, vorbis" <br>* video/mp4; codecs="avc1.4D401E, mp4a.40.2" <br>* video/webm; codecs="vp8.0, vorbis" <br>* audio/ogg; codecs="vorbis" <br>* audio/mp4; codecs="mp4a.40.5"<br>**Note:** 如果包含编解码器，此方法只能返回“probably”。 |

## 技术细节

|  |  |
| ----- | ----- |
| 返回值: | 一个字符串，表示支持级别。 可能的返回值： <br>* `probably` - 最有可能支持 <br>* `maybe` - 可能支持 <br>* "" - （空字符串）不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../../../assets/chrome.svg
[2]: ../../../assets/edge.svg
[3]: ../../../assets/firefox.svg
[4]: ../../../assets/safari.svg
[5]: ../../../assets/opera.svg

