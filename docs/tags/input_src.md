HTML \<input> src 属性
===

## 示例

带有代表提交按钮的图像的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名字:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="image" src="../assets/chrome.svg" alt="Submit" width="48" height="48">
</form>
```

## 定义和用法

`src` 属性指定用作提交按钮的图像的 URL。

**注意：** `src` 属性只能用于（并且是必需的）`<input type="image">`。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| src       | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input src="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定用作提交按钮的图像的 URL。可能的值：<br>* 绝对 URL - 指向另一个网站（如 `src="http://www.example.com/submit.gif"`）<br>* 相对 URL - 指向网站内的文件（如 `src="submit.gif"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


