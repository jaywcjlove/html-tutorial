HTML \<object> Tag
===

## 示例

嵌入图像：

```html idoc:preview:iframe
<object data="../assets/workplace.jpg" width="300" height="200"></object>
```
<!--rehype:style=height: 220px;-->

嵌入的 HTML 页面：

```html idoc:preview:iframe
<object data="./nav.html" width="500" height="200">\</object>
```
<!--rehype:style=height: 240px;-->

嵌入视频：

```html idoc:preview:iframe
<object data="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" width="400" height="280"></object>
```
<!--rehype:style=height: 280px;-->

## 定义和用法

`<object>` 标签定义了一个外部资源的容器。

外部资源可以是网页、图片、媒体播放器或插件应用程序。

要嵌入图片，最好使用`<img>` 标签。

要嵌入 HTML，最好使用 `<iframe>` 标签。

要嵌入视频或音频，最好使用 `<video>` 和 `<audio>` 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<object> | Yes | Yes | Yes | Yes | Yes |

## 插件

`<object>` 标签最初是为嵌入浏览器插件而设计的。

插件是扩展浏览器标准功能的计算机程序。

插件已用于许多不同的目的：

* 运行 Java 小程序
* 运行 ActiveX 控件
* 显示 Flash 电影
* 显示地图
* 扫描病毒
* 验证银行卡号

**警告 ！**

大多数浏览器不再支持 Java 小程序和插件。

任何浏览器都不再支持 ActiveX 控件。

现代浏览器也关闭了对 Shockwave Flash 的支持。

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [data](./object_data.md)     | *URL*         | 指定对象要使用的资源的 URL |
| [form](./object_form.md)     | *form\_id*    | 指定对象属于哪个表单 |
| [height](./object_height.md) | *pixels*      | 指定对象的高度 |
| [name](./object_name.md)     | *name*        | 指定对象的名称 |
| [type](./object_type.md)     | *media\_type* | 指定 data 属性中指定的数据的媒体类型 |
| typemustmatch                   | *true/false*  | 指定类型属性和资源的实际内容是否必须匹配才能显示 |
| [usemap](./object_usemap.md) | *#mapname*    | 指定要与对象一起使用的客户端图像映射的名称 |
| [width](./object_width.md)   | *pixels*      | 指定对象的宽度 |

## 全局属性

`<object>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<object>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Object Element](../tutorial/object.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<menu>` 元素：

```css
object:focus {
  outline: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg