HTML \<embed> type 属性
===

## 示例

具有指定媒体类型的图片：

```html idoc:preview:iframe
<embed
  type="image/png"
  src="../assets/editors-006.png"
>
```
<!--rehype:style=min-height: 200px;-->

## 定义和用法

`type` 属性指定嵌入内容的 Internet 媒体类型（以前称为 MIME 类型）。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| type      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


## 语法

```html
<embed type="media_type">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *media\_type* | 嵌入内容的 Internet 媒体类型。 查看 [IANA 媒体类型](http://www.iana.org/assignments/media-types/) 以获取标准媒体类型的完整列表。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

