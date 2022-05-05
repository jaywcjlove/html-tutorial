HTML `<a>` 标签的 type 属性
===

## 示例

`type` 属性指定链接文档的媒体类型：

```html idoc:preview
<a target="_blank" type="text/html" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

## 定义和用法

`type` 属性指定链接文档的 Internet 媒体类型（以前称为 MIME 类型）。

此属性仅在设置了 [`href`](./a_href.md) 属性时使用。

**注意：** 此属性仅供参考。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| type      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<a type="media_type">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| *media\_type* | 链接文档的 Internet 媒体类型。 查看 [IANA 媒体类型](http://www.iana.org/assignments/media-types/) 以获取标准媒体类型的完整列表。 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
