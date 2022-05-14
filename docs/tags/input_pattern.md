HTML \<input> pattern 属性
===

## 示例

一个 HTML 表单，其输入字段只能包含三个字母（无数字或特殊字符）：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="country_code">国家代码:</label>
  <input type="text" id="country_code" name="country_code"
  pattern="[A-Za-z]{3}" title="三个字母的国家代码"><br><br>
  <input type="submit">
</form>
```

## 定义和使用

`pattern` 属性指定了一个正则表达式，在提交表单时会检查 `<input>` 元素的值。

**注意：** `pattern` 属性适用于以下输入类型：文本、日期、搜索、url、电话、电子邮件和密码。

**提示：** 使用全局 `title` 属性来描述模式以帮助用户。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| pattern   | 5.0 | 10.0 | 4.0 | 10.1 | 9.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input pattern="regexp">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *regexp* | 指定检查 \<input> 元素值的正则表达式 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

`type="password" `的 \<input> 元素必须包含 8 个或更多字符：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="pwd">密码:</label>
  <input type="password" id="pwd" name="pwd"
  pattern=".{8,}" title="八个或更多字符">
  <input type="submit">
</form>
```

一个带有 `type="password"` 的 \<input> 元素，它必须包含 8 个或更多字符，这些字符至少是一个数字和一个大写和小写字母：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="pwd">密码:</label>
  <input type="password" id="pwd" name="pwd"
  pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}"
  title="必须包含至少一个数字和一个大小写字母，以及至少 8 个或更多字符">
  <input type="submit">
</form>
```

`type="email"` 的 \<input> 元素必须按以下顺序排列：`characters@characters.domain`（字符后跟 `@` 符号，后跟更多字符，然后是 "."

之后 ”.” 签名，从 `a` 到 `z` 至少添加 2 个字母：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"
  pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$">
  <input type="submit">
</form>
```

`type="search"` 的 \<input> 元素不能包含以下字符：`'` 或 `"`

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="search">Search:</label>
  <input type="search" id="search" name="search"
  pattern="[^'\x22]+" title="输入无效">
  <input type="submit">
</form>
```

`type="url"` 的 \<input> 元素必须以 `http://` 或 `https://` 开头，后跟至少一个字符：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="website">主页:</label>
  <input type="url" id="website" name="website"
  pattern="https?://.+" title="包括 http://">
  <input type="submit">
</form>
```

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


