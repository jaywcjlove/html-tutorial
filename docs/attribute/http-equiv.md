HTML http-equiv 属性
===

## 定义和用法

`http-equiv` 属性为 `content` 属性的信息/值提供了 HTTP 标头。

`http-equiv` 属性可用于模拟 HTTP 响应标头。

## 适用于

`http-equiv` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<meta>](../tags/meta.md) | [http-equiv](../tags/meta_http_equiv.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

每 30 秒刷新一次文档：

```html
<head>
  <meta http-equiv="refresh" content="30">
</head>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| http-equiv | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg