HTML \<area> rel 属性
===

## 示例

使用 `rel` 属性来指定当前文档和链接文档之间的关系：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area hreflang="en" shape="rect" coords="0,0,82,126" href="a.html" alt="Sun" rel="alternate">
</map>
```

## 定义和用法

`rel` 属性指定当前文档和链接文档之间的关系。

仅在存在 `href` 属性时使用。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| rel       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area rel="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| alternate  | 链接到文档的替代版本（即打印页、翻译或镜像）|
| author     | 指向文档作者的链接|
| bookmark   | 用于书签的永久 URL|
| help       | 帮助文档的链接|
| license    | 文档版权信息的链接|
| next       | 选择中的下一个文档|
| nofollow   | 指向未经认可的文档的链接，例如付费链接。 （Google 使用“nofollow”来指定 Google 搜索爬虫不应跟随该链接）|
| noreferrer | 指定如果用户点击超链接，浏览器不应发送 HTTP 引用标头|
| prefetch   | 指定应缓存目标文档|
| prev       | 选择中的上一个文档|
| search     | 指向文档搜索工具的链接|
| tag        | 当前文档的标签（关键字）|
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg