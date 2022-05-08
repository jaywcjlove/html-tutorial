HTML \<iframe> referrerpolicy 属性
===

## 示例

指定不随请求一起发送推荐人信息：

```html idoc:preview:iframe
<iframe
  src="./iframe.html"
  referrerpolicy="no-referrer"
>

</iframe>
```

## 定义和用法

`referrerpolicy` 属性指定在获取 iframe 时要发送的引荐来源信息。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| referrerpolicy | 51.0 | 79.0 | 50.0 | 11.1 | 38.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<iframe referrerpolicy="no-referrer|no-referrer-when-downgrade|origin|origin-when-cross-origin|same-origin|strict-origin-when-cross-origin|unsafe-url">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| no-referrer                     | 不会随请求一起发送推荐人信息 |
| no-referrer-when-downgrade      | 默认。在没有 HTTPS 的情况下，referrer 标头不会发送到来源 |
| origin                          | 仅向请求客户端发送方案、主机和端口 |
| origin-when-cross-origin        | 对于跨域请求：仅发送方案、主机和端口。对于同源请求：还包括路径 |
| same-origin                     | 对于同源请求：将发送推荐人信息。对于跨域请求：不会发送推荐人信息 |
| strict-origin                   | 如果安全级别相同（例如 HTTPS 到 HTTPS），则仅发送推荐人信息。不要发送到不太安全的目的地（例如 HTTPS 到 HTTP） |
| strict-origin-when-cross-origin | 执行同源请求时发送完整路径。当安全级别保持不变（例如 HTTPS 到 HTTPS）时，仅发送源。不向安全性较低的目的地发送标头（HTTPS 到 HTTP） |
| unsafe-url                      | 发送来源、路径和查询字符串（但不发送片段、密码或用户名）。该值被认为是不安全的 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

