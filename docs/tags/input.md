HTML \<input> 标签
===

## 示例

具有三个输入字段的 HTML 表单； 两个文本字段和一个提交按钮：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```

## 定义和用法

`<input>` 标签指定用户可以输入数据的输入字段。

`<input>` 元素是最重要的表单元素。

`<input>` 元素可以以多种方式显示，具体取决于 type 属性。

不同的输入类型如下：

*   `<input type="button">`
*   `<input type="checkbox">`
*   `<input type="color">`
*   `<input type="date">`
*   `<input type="datetime-local">`
*   `<input type="email">`
*   `<input type="file">`
*   `<input type="hidden">`
*   `<input type="image">`
*   `<input type="month">`
*   `<input type="number">`
*   `<input type="password">`
*   `<input type="radio">`
*   `<input type="range">`
*   `<input type="reset">`
*   `<input type="search">`
*   `<input type="submit">`
*   `<input type="tel">`
*   `<input type="text">` (default value)
*   `<input type="time">`
*   `<input type="url">`
*   `<input type="week">`

查看 [type](./input_type.md) 属性以查看每种输入类型的示例！

## 提示和注意事项

**提示：** 始终使用 [\<label>](./label.md) 标签为 `<input type="text">`、`<input type="checkbox">`、`<input type="radio">`、`<input type="file">` 和 `<input type="password">`。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<input> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [accept](./input_accept.md) | *file\_extension*<br>audio/\*<br>video/\*<br>image/\*<br>*media\_type*  | 指定用户可以从文件输入对话框中选择的文件类型的过滤器（仅适用于 type="file"） |
| [alt](./input_alt.md)                       | *text*   | 指定图像的替代文本（仅适用于 type="image"） |
| [autocomplete](./input_autocomplete.md)     | on<br>off     | 指定 \<input> 元素是否应该启用自动完成功能 |
| [autofocus](./input_autofocus.md)           | autofoc | 指定 \<input> 元素应在页面加载时自动获得焦点 |
| [checked](./input_checked.md)               | checked | 指定在页面加载时应预先选择一个 \<input> 元素（对于 type="checkbox" 或 type="radio"） |
| [dirname](./input_dirname.md)               | *inputname*.dir     | 指定将提交文本方向 |
| [disabled](./input_disabled.md)             | disable | 指定应禁用 \<input> 元素 |
| [form](./input_form.md)                     | *form\_id*    | 指定 \<input> 元素所属的形式 |
| [formaction](./input_formaction.md)         | *URL*    | 指定提交表单时将处理输入控件的文件的 URL（对于 type="submit" 和 type="image"） |
| [formenctype](./input_formenctype.md)       | application/x-www-form-urlencoded<br>multipart/form-data<br>text/plain   | 指定将表单数据提交到服务器时应如何编码（对于 type="submit" 和 type="image"） |
| [formmethod](./input_formmethod.md)         | get post | 定义将数据发送到操作 URL 的 HTTP 方法（对于 type="submit" 和 type="image"） |
| [formnovalidate](./input_formnovalidate.md) | formnovalidate | 定义提交时不应验证表单元素 |
| [formtarget](./input_formtarget.md)         | \_blank<br>\_self<br>\_parent<br>\_top<br>*framename* | 指定在提交表单后显示收到的响应的位置（对于 type="submit" 和 type="image"） |
| [height](./input_height.md)                 | *pixels* | 指定 \<input> 元素的高度（仅适用于 type="image"） |
| [list](./input_list.md)                     | *datalist\_id* | 引用包含 \<input> 元素的预定义选项的 \<datalist> 元素 |
| [max](./input_max.md)                       | *number<br>date* | 指定 \<input> 元素的最大值 |
| [maxlength](./input_maxlength.md)           | *number* | 指定 \<input> 元素中允许的最大字符数 |
| [min](./input_min.md)                       | *number<br>date* | 指定 \<input> 元素的最小值 |
| [minlength](./input_minlength.md)           | *number* | 指定 \<input> 元素中所需的最小字符数 |
| [multiple](./input_multiple.md)             | multiple  | 指定用户可以在 \<input> 元素中输入多个值 |
| [name](./input_name.md)                     | *text* | 指定 \<input> 元素的名称 |
| [pattern](./input_pattern.md)               | *regexp* | 指定检查 \<input> 元素值的正则表达式 |
| [placeholder](./input_placeholder.md)       | *text* | 指定描述 \<input> 元素的预期值的简短提示 |
| [readonly](./input_readonly.md)             | readonly  | 指定输入字段是只读的 |
| [required](./input_required.md)             | required  | 指定在提交表单之前必须填写输入字段 |
| [size](./input_size.md)                     | *number* | 指定 \<input> 元素的宽度（以字符为单位） |
| [src](./input_src.md)                       | *URL* | 指定用作提交按钮的图像的 URL（仅适用于 type="image"） |
| [step](./input_step.md)                     | *number*any  | 指定输入字段中合法数字之间的间隔 |
| [type](./input_type.md)                     | button<br>checkbox<br>color<br>date<br>datetime-local<br>email<br>file<br>hidden<br>image<br>month<br>number<br>password<br>radio<br>range<br>reset<br>search<br>submit<br>tel<br>text<br>time<br>url<br>week  | 指定要显示的类型 \<input> 元素 |
| [value](./input_value.md)                   | *text* | 指定 \<input> 元素的值 |
| [width](./input_width.md)                   | *pixels* | 指定 \<input> 元素的宽度（仅适用于 type="image"） |

## 全局属性

`<input>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<input>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程:

* [HTML Forms](../tutorial/forms.md)
* [HTML Form Elements](../tutorial/form_elements.md)
* [HTML Input Types](../tutorial/form_input_types.md)
* [HTML Input Attributes](../tutorial/form_attributes.md)
* [HTML Input form\* Attributes](../tutorial/form_attributes_form.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg