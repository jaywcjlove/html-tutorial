HTML \<embed> src 属性
===

## 示例

嵌入图片：

```html idoc:preview:iframe
<embed
  src="../assets/editors-006.png"
>
```
<!--rehype:style=min-height: 200px;-->

## 定义和用法

`src` 属性指定要嵌入的外部文件的地址。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| src       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<embed src="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定要嵌入的外部文件的地址。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `href="http://www.example.com/hello.swf"`） <br>* 相对 URL - 指向网站内的文件（如 `href="hello.swf"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
