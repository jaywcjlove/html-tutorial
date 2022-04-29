HTML \<form> 标签
===


## 示例

具有两个输入字段和一个提交按钮的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <label for="fname">名:</label>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">姓:</label>
  <input type="text" id="lname" name="lname"><br>
  <input type="submit" value="提交">
</form>
```
## 定义和用法

`<form>` 标签用于为用户输入创建 HTML 表单。

`<form>` 元素可以包含以下一个或多个表单元素：

*   [\<input>](./input.md)
*   [\<textarea>](./textarea.md)
*   [\<button>](./button.md)
*   [\<select>](./select.md)
*   [\<option>](./option.md)
*   [\<optgroup>](./optgroup.md)
*   [\<fieldset>](./fieldset.md)
*   [\<label>](./label.md)
*   [\<output>](./output.md)

## Browser Support

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<form> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [accept-charset](./form_accept_charset.md) | *character\_set* | 指定要用于表单提交的字符编码|
| [action](./form_action.md)                 | *URL* | 指定提交表单时将表单数据发送到何处|
| [autocomplete](./form_autocomplete.md)     | on off  | 指定表单是否应该打开或关闭自动完成功能|
| [enctype](./form_enctype.md) | _application/x-www-form-urlencoded_<br >multipart/form-data<br >text/plain  | 指定将表单数据提交到服务器时应如何编码（仅适用于 method="post"）|
| [method](./form_method.md) | get<br >post  | 指定发送表单数据时使用的 HTTP 方法|
| [name](./form_name.md)                     | *text* | 指定表单的名称|
| [novalidate](./form_novalidate.md)         | novalidate  | 指定提交时不应验证表单|
| [rel](./form_rel.md)                       | external<br >help<br >license<br >next<br >nofollow<br >noopener<br >noreferrer<br >opener<br >prev<br >search  | 指定链接资源和当前文档之间的关系|
| [target](./form_target.md)                 | \_blank<br >\_self<br >\_parent<br >\_top  | 指定在哪里显示提交表单后收到的响应|

## 全局属性

`<form>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<form>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

带有复选框的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <input type="checkbox" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" name="vehicle3" value="Boat" checked>
  <label for="vehicle3"> I have a boat</label><br><br>
  <input type="submit" value="Submit">
</form>
```

带有单选按钮的 HTML 表单：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS" checked="checked">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<form>` 元素：

```css
form {
  display: block;
  margin-top: 0em;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg