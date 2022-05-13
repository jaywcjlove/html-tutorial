HTML \<input> formmethod 属性
===

## 示例

第二个提交按钮覆盖表单的 HTTP 方法：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="提交">
  <input type="submit" formmethod="post" value="使用 POST 提交">
</form>
```

## 定义和用法

`formmethod` 属性定义了将表单数据发送到操作 URL 的 HTTP 方法。

`formmethod` 属性覆盖了 `<form>` 元素的 `method` 属性。

**注意：** `formmethod` 属性可以与 `type="submit"` 和 `type="image"` 一起使用。

表单数据可以作为 URL 变量（`method="get"`）或作为 HTTP post 事务（`method="post"`）发送。

**关于“get”方法的注意事项：**

* 此方法以名称/值对的形式将表单数据附加到 URL
* 此方法对于用户想要为结果添加书签的表单提交很有用
* 您可以在 URL 中放置多少数据是有限制的（因浏览器而异），因此，您无法确定所有表单数据都会正确传输
* 切勿使用“get”方法传递敏感信息！ （密码或其他敏感信息将显示在浏览器的地址栏中）

**关于“post”方法的注意事项：**

* 此方法将表单数据作为 HTTP 发布事务发送
* 使用“post”方式提交的表单无法添加书签
* "post" 方法比 "get" 更健壮和安全，并且 "post" 没有大小限制

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| formmethod | Yes | 10.0 | Yes | 5.1 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<input formmethod="get|post">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| get   | 默认。 以名称`/`值对的形式将表单数据附加到 URL： `URL?name=value&name=value` |
| post  | 将表单数据作为 HTTP 发布事务发送 |
<!--rehype:style=width: 100%; display: inline-table;-->

[HTML \<input> tag](./input.md "HTML input 标签参考")

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

