HTML \<area> media 属性
===

## 示例

使用 `media` 属性来指定目标 `URL` 优化的媒体/设备：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126"
    media="screen and (min-color-index:256)" href="../tags/a.html" alt="Sun">
  <area shape="circle" coords="90,58,3"
    media="screen and (min-color-index:256)" href="../tags/address.html" alt="Mercury">
  <area shape="circle" coords="124,58,8"
    media="screen and (min-color-index:256)" href="../tags/applet.html" alt="Venus">
</map>
```

## 定义和用法

`media` 属性指定目标 URL 优化的媒体/设备。

此属性用于指定 URL 是为特殊设备（如 iPhone）、语音或印刷媒体设计的。

该属性可以接受多个值。

仅在存在 `href` 属性时使用。

**注意：** 此属性仅供参考。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| media     | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area media="value">
```

## 可能的运算符

| 值 Value | 描述 Description |
| ----- | ----- |
| and   | 指定 AND 运算符 |
| not   | 指定 NOT 运算符 |
| ,     | 指定 OR 运算符 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 设备

| 值 Value | 描述 Description |
| ----- | ----- |
| all        | 默认。 适用于所有设备 |
| aural      | 语音合成器 |
| braille    | 盲文反馈装置 |
| handheld   | 手持设备（小屏幕，有限带宽） |
| projection | 投影仪 |
| print      | 打印预览模式/打印页面 |
| screen     | 电脑屏幕 |
| tty        | 使用固定间距字符网格的电传打字机和类似媒体 |
| tv         | 电视类型的设备（低分辨率，有限的滚动能力） |
<!--rehype:style=width: 100%; display: inline-table;-->

## 值

| 值 Value | 描述 Description |
| ----- | ----- |
| width               | 指定目标显示区域的宽度。可以使用“min-”和“max-”前缀。示例：media="screen and (min-width:500px)" |
| height              | 指定目标显示区域的高度。可以使用“min-”和“max-”前缀。示例：media="screen and (max-height:700px)" |
| device-width        | 指定目标显示器/纸张的宽度。可以使用“min-”和“max-”前缀。示例：media="screen and (device-width:500px)" |
| device-height       | 指定目标显示器/纸张的高度。可以使用“min-”和“max-”前缀。示例：media="screen and (device-height:500px)" |
| orientation         | 指定目标显示器/纸张的方向。可能的值：“portrait”或“landscape” 示例：media="all and (orientation:landscape)" |
| aspect-ratio        | 指定目标显示区域的宽高比。可以使用“min-”和“max-”前缀。示例：media="screen and (aspect-ratio:16/9)" |
| device-aspect-ratio | 指定目标显示器/纸张的设备宽度/设备高度比率。可以使用“min-”和“max-”前缀。示例：media="screen and (aspect-ratio:16/9)" |
| color               | 指定目标显示器的每种颜色的位数。可以使用“min-”和“max-”前缀。示例：media="screen and (color:3)" |
| color-index         | 指定目标显示器可以处理的颜色数。可以使用“min-”和“max-”前缀。示例：media="screen and (min-color-index:256)" |
| monochrome          | 指定单色帧缓冲区中每像素的位数。可以使用“min-”和“max-”前缀。示例：media="screen and (monochrome:2)" |
| resolution          | 指定目标显示器/纸张的像素密度（dpi 或 dpcm）。可以使用“min-”和“max-”前缀。示例：media="打印和（分辨率：300dpi）" |
| scan                | 指定电视显示器的扫描方法。可能的值是“渐进式”和“隔行式”。示例：media="tv and (scan:interlace)" |
| grid                | 指定输出设备是网格还是位图。网格的可能值为“1”，否则为“0”。示例：media="handheld and (grid:1)" |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg