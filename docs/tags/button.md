HTML \<button> 标签
===

## 示例

一个可点击的按钮标记如下：

```HTML idoc:preview
<button type="button">Click Me!</button>
```

## 定义和用法

`<button>` 标签定义了一个可点击的按钮。

在 `<button>` 元素中，您可以放置文本（以及 `<i>`、`<b>`、`<strong>`、`<br>`、`<img>` 等标签）。 使用 `<input>` 元素创建的按钮是不可能的！

**提示：** 始终为 `<button>` 元素指定 `type` 属性，以告诉浏览器它是什么类型的按钮。

**提示：** 您可以使用 CSS 轻松设置按钮样式！

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<button> | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [autofocus](./button_autofocus.md) | autofocus | 指定当页面加载时按钮应该自动获得焦点|
| [disabled](./button_disabled.md) | disabled | 指定应禁用按钮|
| [form](./button_form.md) | *form\_id* | 指定按钮属于哪个表单|
| [formaction](./button_formaction.md) | *URL* | 指定提交表单时将表单数据发送到何处。仅适用于 type="submit"|
| [formenctype](./button_formenctype.md) | application/x-www-form-urlencoded<br/>multipart/form-data text/plain | 指定表单数据在发送到服务器之前应如何编码。仅适用于 type="submit"|
| [formmethod](./button_formmethod.md) | get<br/>post | 指定如何发送表单数据（使用哪种 HTTP 方法）。仅适用于 type="submit"|
| [formnovalidate](./button_formnovalidate.md) | formnovalidate | 指定不应在提交时验证表单数据。仅适用于 type="submit"|
| [formtarget](./button_formtarget.md) | \_blank<br/>\_self<br/>\_parent<br/>\_top<br/>*framename* | 指定提交表单后显示响应的位置。仅适用于 type="submit"|
| [name](./button_name.md) | *name* | 指定按钮的名称|
| [type](./button_type.md) | button<br/>reset<br/>submit | 指定按钮的类型|
| [value](./button_value.md) | *text* | 指定按钮的初始值|
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<button>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<button>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

使用 CSS 设置按钮样式：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <style>
    .button { border: none; color: white; padding: 15px 32px; text-align: center; text-decoration: none; display: inline-block; font-size: 16px; margin: 4px 2px; cursor: pointer; }
    .button1 {background-color: #4CAF50;}
    .button2 {background-color: #008CBA;}
  </style>
</head>
<body>
  <button class="button button1">Green</button> <button class="button button2">Blue</button>
</body>
</html>
```

使用 CSS 设置按钮样式（带有悬停效果）：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <style>
  .button { border: none; color: white; padding: 16px 32px; text-align: center; text-decoration: none; display: inline-block; font-size: 16px; margin: 4px 2px; transition-duration: 0.4s; cursor: pointer; }
  .button1 { background-color: white; color: black; border: 2px solid #4CAF50; }
  .button1:hover { background-color: #4CAF50; color: white; }
  .button2 { background-color: white; color: black; border: 2px solid #008CBA; }
  .button2:hover { background-color: #008CBA; color: white; }
  </style>
</head>
<body>
  <button class="button button1">Green</button> <button class="button button2">Blue</button>
</body>
</html>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg