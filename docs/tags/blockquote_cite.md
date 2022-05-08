HTML \<blockquote> cite 标签
===

## 示例

从另一个来源引用的部分：

```html idoc:preview:iframe
<blockquote cite="http://www.worldwildlife.org/who/index.html">
50 年来，WWF 一直在保护自然的未来。 作为世界领先的保护组织，WWF 在 100 个国家开展工作，并得到美国 120 万会员和全球近 500 万会员的支持。
</blockquote>
```

## 定义和用法

`cite` 属性指定引用的来源。

**提示：** 如果有的话，总是添加引用的来源是一个好习惯。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| cite      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

`cite` 属性在任何主要浏览器中都不会呈现为任何特殊内容，但搜索引擎可以使用它来获取有关报价的更多信息。

## 语法

```html
<blockquote cite="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 引用的来源。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `cite="http://www.example.com/page.htm"`） <br>* 相对 URL - 指向网站内的文件（如 `cite="page.htm"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg