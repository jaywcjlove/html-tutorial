HTML \<param> 标签
===

## 示例

将 `autoplay` 参数设置为 `true`，这样声音就会在页面加载后立即开始播放：

```html idoc:preview:iframe
<object data="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">
  <param name="autoplay" value="true">
</object>
```
<!--rehype:style=height: 180px;-->

## 定义和用法

`<param>` 标签用于定义 [\<object>](./object.md) 元素的参数。

## 浏览器支持

所有主流浏览器都支持 `<param>` 标签。 但是，并非所有浏览器都支持 [\<object>](./object.md) 中定义的文件格式。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<param> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [name](./param_name.md)   | *name*  | 指定参数的名称 |
| [value](./param_value.md) | *value* | 指定参数的值 |

## 全局属性

`<param>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<param>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<param>` 元素：

```css
param {
  display: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg