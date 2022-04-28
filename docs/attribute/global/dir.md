HTML dir 属性
===

`dir` 属性指定元素内容的文本方向。

## 实例

具有从右到左方向的段落：

```html idoc:preview
<p dir="rtl">Write this text right-to-left!</p>
```

## 定义和使用

`dir` 属性指定元素内容的文本方向。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;dir&gt;__ | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<element dir="ltr|rtl|auto">
```

## 属性值

值 Value | 描述 Description
---- | ----
ltr | 默认。 从左到右的文本方向
rtl | 从右到左的文本方向
auto | 让浏览器根据内容判断文本方向（仅在文本方向未知时推荐）


[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg