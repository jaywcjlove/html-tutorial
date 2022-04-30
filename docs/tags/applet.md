HTML \<applet> 标签
===

[![](https://shields.io/badge/HTML5-已弃用/过时-yellow?logo=HTML5)](https://caniuse.com/?search=<applet>)

`<applet>` 标签在 HTML 4 中用于定义嵌入式 `applet`（插件）。

## 插件

插件是扩展浏览器标准功能的计算机程序。

插件已用于许多不同的目的：

- 运行 Java 小程序
- 运行 ActiveX 控件
- 显示 Flash 影片
- 显示地图
- 扫描病毒
- 验证银行 ID

> 大多数浏览器不再支持 `Java Applets` 和插件。  
> 任何浏览器都不再支持 `ActiveX` 控件。  
> 现代浏览器也关闭了对 `Shockwave Flash` 的支持。
<!--rehype:style=background: #ffffcc; padding: 10px 0 10px 15px; border-left: 4px solid #f4cc41;-->

## 改用什么？

如果要嵌入视频，请使用 [\<video>](../tags/video.md) 标签：

## 更多示例

如果要嵌入视频，请使用 [\<video>](../tags/video.md) 标签：

```html idoc:preview
<video width="320" controls>
  <source type="video/mp4" src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <source type="video/webm" src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">
  Your browser does not support the video tag.
</video>
```

如果要嵌入音频，请使用 [\<audio>](../tags/audio.md) 标签：

```html idoc:preview
<audio controls>
  <source type="audio/ogg" src="horse.ogg">
  <source type="audio/mpeg" src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3">
  Your browser does not support the audio tag.
</audio>
```