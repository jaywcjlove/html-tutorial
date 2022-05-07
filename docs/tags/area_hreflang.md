HTML \<area> hreflang 属性
===

## 示例

使用 `hreflang` 属性为图像映射中的每个区域指定目标 `URL` 的语言：

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

`hreflang` 属性指定区域中目标 URL 的语言。

此属性仅在设置了 `href` 属性时使用。

**注意：** 此属性仅供参考。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| hreflang  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<area hreflang="language_code">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *language\_code* | 一个由两个字母组成的语言代码，用于指定链接文档的语言。 要查看所有可用的语言代码，请访问我们的 [语言代码参考](../reference/language_codes.md)。 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg