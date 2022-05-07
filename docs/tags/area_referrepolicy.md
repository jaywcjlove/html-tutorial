HTML \<area> referrerpolicy 属性
===

## 示例

为区域超链接设置 `referrerpolicy` 属性：

```html idoc:preview
<img src="../assets/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area referrerpolicy="same-origin" shape="rect" coords="34,44,270,350" alt="Computer" href="a.html">
  <area referrerpolicy="same-origin" shape="rect" coords="290,172,333,250" alt="Phone" href="abbr.html">
  <area referrerpolicy="same-origin" shape="circle" coords="337,300,44" alt="Cup of coffee" href="address.html">
</map>
```
<!--rehype:style=min-height: 280px;-->

## 定义和用法

`referrerpolicy` 属性指定当用户点击超链接时要发送哪些推荐人信息。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| referrerpolicy | 51.0 | 79.0 | 50.0 | 11.1 | 38.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area referrerpolicy="no-referrer|no-referrer-when-downgrade|origin|origin-when-cross-origin|same-origin|strict-origin-when-cross-origin|unsafe-url">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| no-referrer                     | 不发送推荐人信息|
| no-referrer-when-downgrade      | 默认。如果协议安全级别保持不变或更高（HTTP 到 HTTP、HTTPS 到 HTTPS、HTTP 到 HTTPS 可以），则发送源、路径和查询字符串。不发送任何安全级别较低的内容（HTTPS 到 HTTP 不行）|
| origin                          | 发送文档的来源（方案、主机和端口）|
| origin-when-cross-origin        | 为跨域请求发送文档的来源。发送同源请求的源、路径和查询字符串|
| same-origin                     | 发送同源请求的引用者。跨域请求不发送推荐人|
| strict-origin-when-cross-origin | 如果协议安全级别保持不变或更高（HTTP 到 HTTP、HTTPS 到 HTTPS 和 HTTP 到 HTTPS 都可以），则发送源。不发送任何安全级别较低的内容（HTTPS 到 HTTP）|
| unsafe-url                      | 发送源、路径和查询字符串（不考虑安全性）。小心使用这个值！|
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg