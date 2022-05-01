HTML \<ruby> Tag
===

## 示例

ruby 标注：

```html idoc:preview
<ruby>
漢 <rt>han</rt>
</ruby>
```

## 定义和用法

`<ruby>` 标签指定了一个 ruby 注释。

ruby 标注 是一个小的额外文本，附加到正文以指示相应字符的发音或含义。 这种注释在日本出版物中经常使用。

将 `<ruby>` 与 [\<rt>](./rt.md) 和 [\<rp>](./rp.md) 一起使用：`<ruby>` 元素由一个或多个字符组成 需要一个解释/发音，以及一个提供该信息的 [\<rt>](./rt.md) 元素，以及一个可选的 [\<rp>](./rp.md) 元素，用于定义为不支持 ruby 注释的浏览器显示的内容。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<ruby> | 5.0 | 5.5 | 38.0 | 5.0 | 15.0 |

## 全局属性

`<ruby>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<ruby>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg