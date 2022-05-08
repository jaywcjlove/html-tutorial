HTML \<img> referrerpolicy 属性
===

## 示例

设置图片的 `referrerpolicy`：

```html idoc:preview
<img src="../assets/chrome.svg" alt="Some image" referrerpolicy="no-referrer">
```

## 定义和用法

`referrerpolicy` 属性指定在获取图像时要使用的引荐来源信息。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| referrerpolicy | 51.0 | 79.0 | 50.0 | 11.1 | 38.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img referrerpolicy="no-referrer|no-referrer-when-downgrade|origin|origin-when-cross-origin|unsafe-url">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| no-referrer                | 不发送推荐人信息 |
| no-referrer-when-downgrade | 默认。 在没有 HTTPS 的情况下，referrer 标头不会发送到来源 |
| origin                     | 发送文档的来源（方案、主机和端口） |
| origin-when-cross-origin   | 对于跨域请求：仅发送方案、主机和端口。 对于同源请求：还包括路径 |
| unsafe-url                 | 发送来源、路径和查询字符串（但不发送片段、密码或用户名）。 该值被认为是不安全的 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg