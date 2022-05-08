HTML \<img> longdesc 属性
===

## 示例

如何使用 `longdesc` 属性的几个示例：

```html idoc:preview
<!-- 描述与图像在同一页上 -->
<img src="../assets/chrome.svg" alt="W3Schools.com" width="100" height="132" longdesc="#w3htmlExplained">

<!-- 描述在外部页面中 -->
<img src="../assets/chrome.svg" alt="W3Schools.com" width="100" height="132" longdesc="w3html.txt">

<!-- 描述是外部页面中的几个之一 -->
<img src="../assets/chrome.svg" alt="W3Schools.com" width="100" height="132" longdesc="http://example.com/desc#item3">

<!-- 描述包含在 data:URI 中 -->
<img src="../assets/chrome.svg" alt="W3Schools.com" width="100" height="132" longdesc="data%3Atext%2Fhtml%3Bcharset%3Dutf-8%3B%2C%3C%21DOCTYPE%20html%3E%3Chtml%3E%3Chead%3E%3Ctitle%3E%E6%A0%87%E5%BF%97%E8%AF%B4%E6%98%8E%3C%2Ftitle%3E%3C%2Fhead%3E%3Cbody%3E%3Cp%3E%E4%B8%80%E4%BA%9B%E6%8F%8F%E8%BF%B0%E5%9C%A8%E8%BF%99%E9%87%8C%3C%2Fp%3E%3C%2Fbody%3E%3C%2Fhtml%3E">
```

## 定义和用法

`longdesc` 属性指定了一个指向图像详细描述的超链接。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| longdesc  | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<img longdesc="string">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *string* | 指向图像详细描述的超链接。可能的值：<br>* 指向另一个元素的 id <br>* 绝对 URL - 指向另一个网站（如 `longdesc="http://www.example.com/description.txt"`） <br>* 相对 URL - 指向网站内的文件（如 `longdesc="description.txt"`） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
