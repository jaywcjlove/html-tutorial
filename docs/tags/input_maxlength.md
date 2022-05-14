HTML \<input> maxlength 属性
===

## 示例

最大长度为 10 个字符的 \<input> 元素：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="username">用户名:</label>
  <input type="text" id="username" name="username" maxlength="10"><br><br>
  <input type="submit" value="提交">
</form>
```

## 定义和用法

`maxlength` 属性指定 `<input>` 元素中允许的最大字符数。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| maxlength | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input maxlength="number">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *number* | \<input> 元素中允许的最大字符数。 默认值为 `524288` |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
