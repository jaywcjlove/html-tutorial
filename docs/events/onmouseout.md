HTML onmouseout 事件属性
===

当鼠标指针移出元素时触发

## 示例

将鼠标指针移出图像时执行 JavaScript：

```html idoc:preview:iframe
<img onmouseover="bigImg(this)" onmouseout="normalImg(this)" border="0" src="../assets/chrome.svg" width="32" height="32">
<p>当用户将鼠标悬停在图像上时会触发函数 bigImg()。 此功能可放大图像。</p>
<p>当鼠标指针移出图像时触发函数 normalImg()。 该函数将图像的高度和宽度设置回正常值。</p>
<script>
function bigImg(x) {
  x.style.height = "64px";
  x.style.width = "64px";
}
function normalImg(x) {
  x.style.height = "32px";
  x.style.width = "32px";
}
</script>
```

```html
<img onmouseout="normalImg(this)" src="../assets/chrome.svg">
```

## 定义和使用

当鼠标指针移出元素时触发 onmouseout 属性。

**提示：** onmouseout 属性通常与 [onmouseover](./onmouseover.md) 属性一起使用。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onmouseout | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onmouseout="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 onmouseout 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: [\<base>](../tags/base.md), [\<bdo>](../tags/bdo.md), [\<br>](../tags/br.md), [\<head>](../tags/head.md), [\<html>](../tags/html.md), [\<iframe>](../tags/iframe.md), [\<meta>](../tags/meta.md), [\<param>](../tags/param.md), [\<script>](../tags/script.md), [\<style>](../tags/style.md), 和 [\<title>](../tags/title.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
