HTML \<rp> Tag
===

## 示例

ruby 标注：

```html idoc:preview
<ruby>
漢 <rp>(</rp><rt>han</rt><rp>)</rp>
</ruby>
```

## 定义和用法

`<rp>` 标签可用于在 ruby 文本周围提供括号，由不支持 ruby 注释的浏览器显示。

将 `<rp>` 与 [<ruby>](./ruby.md) 和 [\<rt>](./rt.md) 一起使用：[<ruby>](./ruby.md) 元素由一个或多个需要 解释/发音，以及提供该信息的 [\<rt>](./rt.md) 元素，以及一个可选的 [`<rp>`](./rp.md) 元素，用于定义为不支持 ruby 注释的浏览器显示的内容。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<rp>   | 5.0 | 5.5 | 38.0 | 5.0 | 15.0 |

## 全局属性

`<rp>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<rp>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg