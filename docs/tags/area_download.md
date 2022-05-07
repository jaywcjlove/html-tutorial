HTML \<area> download 属性
===

## 示例

使用 `download` 属性指定当用户单击超链接时将下载目标：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area download shape="rect" coords="0,0,82,126" href="a.html" alt="Sun">
  <area download shape="circle" coords="90,58,3" href="address.html" alt="Mercury">
  <area download shape="circle" coords="124,58,8" href="applet.html" alt="Venus">
</map>
```

## 定义和用法

`download` 属性指定当用户单击超链接时将下载目标（`href` 属性中指定的文件）。

`download` 属性的可选值将是文件下载后的新名称。 对允许值没有限制，浏览器会自动检测正确的文件扩展名并将其添加到文件中（`.img`、`.pdf`、`.txt`、`.html` 等）。

如果省略该值，则使用原始文件名。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| download  | 14.0\* | 18.0 | 20.0\* | 10.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

\* Chrome 65+ 和 Firefox 仅支持同源下载链接。

## 语法

```html
<area download="filename">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *filename* | 可选的。 指定下载文件的新文件名 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

为下载属性指定一个值，它将是下载文件的新文件名（`sun.html` 而不是 `a.html` 等）：

```html idoc:preview
<img src="https://user-images.githubusercontent.com/1680273/165700877-949e520a-c085-40ce-abd4-2996da31f33b.png" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap">
  <area download="sun" shape="rect" coords="0,0,82,126" href="a.html" alt="Sun">
  <area download shape="circle" coords="90,58,3" href="address.html" alt="Mercury">
  <area download shape="circle" coords="124,58,8" href="applet.html" alt="Venus">
</map>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg