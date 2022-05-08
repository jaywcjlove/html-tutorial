HTML \<button> formmethod 属性
===

## 示例

带有两个提交按钮的表单。 第一个提交按钮用 `method="get"` 提交表单数据，第二个用 `method="post"` 提交表单数据：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <button type="submit">Submit</button>
  <button type="submit" formmethod="post">Submit using POST</button>
</form>
```

## 定义和用法

`formmethod` 属性指定发送表单数据时使用的 HTTP 方法。此属性覆盖表单的“方法”属性。

`formmethod` 属性仅用于具有 `type="submit"` 的按钮。

表单数据可以作为 URL 变量（使用 `method="get"`）或作为 HTTP post（使用 `method="post"`）发送。

`get` 方法的注意事项：

* 它以名称/值对的形式将表单数据附加到 URL
* 这对于用户想要为结果添加书签的表单提交很有用
* 您可以在 `URL` 中放置多少数据是有限制的（因浏览器而异），因此，您无法确定所有表单数据都会正确传输
* 切勿使用 `get` 方法传递敏感信息！ （密码或其他敏感信息将显示在浏览器的地址栏中）

关于 `post` 方法的注意事项：

* 它将表单数据作为 HTTP 发布事务发送
* 使用 `post` 方式提交的表单无法添加书签
* 它比 `get` 更健壮和安全
* 它没有尺寸限制

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| formmethod | 9.0 | 10.0 | 4.0 | 5.1 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<button type="submit" formmethod="get|post">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| get   | 将表单数据附加到 URL： `URL?name=value\&name=value` |
| post  | 将表单数据作为 HTTP 发布事务发送 |
<!--rehype:style=width: 100%; display: inline-table;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
