HTML \<input> formaction 属性
===

## 示例

具有两个提交按钮的 HTML 表单，具有不同的操作：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="提交">
  <input type="submit" formaction="/action_page2.php" value="提交到另一个页面">
</form>
```

## 定义和用法

`formaction` 属性指定提交表单时将处理输入控件的文件的 URL。

`formaction` 属性覆盖了 `<form>` 元素的 `action` 属性。

**注意：** `formaction` 属性与 `type="submit"` 和 `type="image"` 一起使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| formaction | Yes | 10.0 | Yes | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input formaction="URL">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *URL* | 指定提交表单时将处理输入控件的文件的 URL。可能的值：<br>* 绝对 URL - 页面的完整地址（如 `href="http://www.example.com/formresult.asp"`)<br>* 相对 URL - 指向当前站点中的文件（如 `href="formresult.asp"`） |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

