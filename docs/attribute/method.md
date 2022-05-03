HTML method 属性
===

## 定义和用法

`method` 属性指定如何发送表单数据（表单数据被发送到 `action` 属性中指定的页面）。

表单数据可以作为 URL 变量（使用 `method="get"`）或作为 HTTP 发布事务（使用 `method="post"`）发送。

**关于 GET 的注意事项：**

* 以名称/值对的形式将表单数据附加到 URL 中
* URL 的长度是有限的（大约 3000 个字符）
* 切勿使用 GET 发送敏感数据！ （将在 URL 中可见）
* 对于用户想要为结果添加书签的表单提交很有用
* GET 更适合非安全数据，例如 Google 中的查询字符串

**关于 POST 的注意事项：**

* 在 HTTP 请求的正文中附加 form-data（数据未显示在 URL 中）
* 没有大小限制
* 不能为 POST 提交的表单添加书签

## 适用于

`method` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<form>](../tags/form.md) | [method](../tags/form_method.md) |

## 示例

使用“get”方法提交表单：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| method    | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg