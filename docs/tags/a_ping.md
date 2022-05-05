HTML `<a>` 标签的 ping 属性
===

## 示例

当用户点击链接时通知 `example.com/trackpings`：

```html
<a href="https://www.example.com/html" ping="https://www.example.com/trackpings">
  点击链接时通知 `example.com/trackpings`
</a>
```

## 定义和用法

`ping` 属性指定了在用户点击超链接时要通知的 URL 列表。

当用户点击超链接时，`ping` 属性会向指定的 URL 发送一个简短的 HTTP POST 请求。

此属性对于监视/跟踪很有用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| ping      | Yes | No | Yes | No | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<a ping="*URL"*>
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| *URL* | 指定用户点击超链接时要通知的 URL。 必须是一个或多个有效 URL 的空格分隔列表 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg