HTML \<label> Tag
===

## 示例

Three radio buttons with labels:

```html idoc:preview:iframe
<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form>
```

## 定义和用法

The `<label>` tag defines a label for several elements:

* [\<input type="checkbox">](./input_type_checkbox.md)
* [\<input type="color">](./input_type_color.md)
* [\<input type="date">](./input_type_date.md)
* [\<input type="datetime-local">](./input_type_datetime-local.md)
* [\<input type="email">](./input_type_email.md)
* [\<input type="file">](./input_type_file.md)
* [\<input type="month">](./input_type_month.md)
* [\<input type="number">](./input_type_number.md)
* [\<input type="password">](./input_type_password.md)
* [\<input type="radio">](./input_type_radio.md)
* [\<input type="range">](./input_type_range.md)
* [\<input type="search">](./input_type_search.md)
* [\<input type="tel">](./input_type_tel.md)
* [\<input type="text">](./input_type_text.md)
* [\<input type="time">](./input_type_time.md)
* [\<input type="url">](./input_type_url.md)
* [\<input type="week">](./input_type_week.md)
* [\<meter>](./meter.md)
* [\<progress>](./progress.md)
* [\<select>](./select.md)
* [\<textarea>](./textarea.md)

正确使用具有上述元素的标签将受益：

* 屏幕阅读器用户（当用户专注于元素时，将大声读出标签）
* 难以点击非常小的区域（例如复选框）的用户 - 因为当用户点击 `<label>` 元素中的文本时，它会切换输入（这会增加点击区域）。

## 提示和注意事项

**提示：** `<label>` 的 for 属性必须等于相关元素的 id 属性才能将它们绑定在一起。 也可以通过将元素放置在 `<label>` 元素中来将标签绑定到元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<label> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [for](./label_for.md)   | *element\_id* | 指定标签应绑定到的表单元素的 id |
| [form](./label_form.md) | *form\_id*    | 指定标签属于哪个表单 |

## 全局属性

`<label>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<label>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<label>` 元素：

```css
label {
  cursor: default;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg