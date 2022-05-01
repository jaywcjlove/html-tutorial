HTML \<rt> Tag
===

## 示例

ruby 注释：

```html idoc:preview
<ruby>
漢 <rt> han </rt>
</ruby>
```

## 定义和用法

`<rt>` 标签在 ruby 注释中定义字符的解释或发音（对于东亚字体）。

将 `<rt>` 与 [\<ruby>](./ruby.md) 和 [\<rp>](./rp.md) 一起使用：\<ruby> 元素由一个或多个字符组成 一个解释/发音，和一个提供该信息的 [`<rt>`](./rt.md) 元素，以及一个可选的[\<rp>](./rp.md) 元素，它定义了为不支持 ruby 注释的浏览器显示的内容。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<rt>   | 5.0 | 5.5 | 38.0 | 5.0 | 15.0 |

## 全局属性

`<rt>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<rt>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<rt>` 元素：

```css
rt {
  line-height: normal;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg