HTML \<input> required 属性
===

## 示例

具有必需输入字段的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="username">用户名:</label>
  <input type="text" id="username" name="username" required>
  <input type="submit">
</form>
```

## 定义和用法

`required` 属性是一个布尔属性。

如果存在，它指定在提交表单之前必须填写输入字段。

**注意：** `required` 属性适用于以下输入类型：`text`, `search`, `url`, `tel`, `email`, `password`, `date pickers`, `number`, `checkbox`, `radio`, 和 `file`。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| required  | 5.0 | 10.0 | 4.0 | 10.1 | 9.6 |

## 语法

```html
<input required>
```