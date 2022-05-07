HTML \<area> type 属性
===

## 示例

使用 `type` 属性指定目标 `URL` 的 `MIME` 类型：

```html idoc:preview
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="../assets/workplace.jpg" type="image/jpg">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```

## 定义和用法

`type` 属性指定目标 URL 的 Internet 媒体类型（以前称为 MIME 类型）。

此属性仅在设置了 `href` 属性时使用。

**注意：** 此属性仅供参考。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| type      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area type="media_type">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *media\_type* | 链接文档的 Internet 媒体类型。 查看 [IANA 媒体类型](http://www.iana.org/assignments/media-types/) 以获取标准媒体类型的完整列表。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg