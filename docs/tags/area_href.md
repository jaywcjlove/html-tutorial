HTML \<area> href 属性
===

## 示例

使用 href 属性为图像映射中的每个区域指定链接目标：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area hreflang="en" shape="rect" coords="0,0,82,126" href="a.html" alt="Sun">
  <area hreflang="en" shape="circle" coords="90,58,3" href="address.html" alt="Mercury">
  <area hreflang="en" shape="circle" coords="124,58,8" href="applet.html" alt="Venus">
</map>
```

## 定义和用法

`href` 属性指定区域的超链接目标。

如果 `href` 属性不存在，则 `<area>` 标签不是超链接。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| href      | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area href="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定区域的超链接目标。可能的值：* 绝对 URL - 指向另一个网站（如 `href="http://www.example.com/sun.htm"`）<br>* 相对 URL - 指向网站内的文件（如 `href="sun.htm"`）<br> * 链接到页面内具有指定 id 的元素（如 `href="#top"`）<br>* 其他协议（如 `https://`、`ftp://`、`mailto:`、`file:` 等）<br>* 一个脚本（比如 `href="javascript:alert('Hello');"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg