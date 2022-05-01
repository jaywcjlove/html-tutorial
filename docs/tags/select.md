HTML \<select> Tag
===

## 示例

创建一个包含四个选项的下拉列表：

```html idoc:preview:iframe
<label for="cars">Choose a car:</label>
<select name="cars" id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="mercedes">Mercedes</option>
  <option value="audi">Audi</option>
</select>
```
<!--rehype:style=height: 90px;-->

## 定义和用法

`<select>` 元素用于创建下拉列表。

`<select>` 元素最常用于表单中，用于收集用户输入。

表单提交后需要 name 属性引用表单数据（如果省略name属性，下拉列表中的数据将不会被提交）。

需要 `id` 属性来将下拉列表与标签相关联。

`<select>` 元素内的 [\<option>](./option.md) 标记定义下拉列表中的可用选项。

**提示：** 始终添加 [\<label>](./label.md) 标记以获得最佳可访问性实践！

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<select> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [autofocus](./select_autofocus.md) | autofocus  | 指定当页面加载时下拉列表应该自动获得焦点 |
| [disabled](./select_disabled.md)   | disabled   | 指定应禁用下拉列表 |
| [form](./select_form.md)           | *form\_id* | 定义下拉列表属于哪个表单 |
| [multiple](./select_multiple.md)   | multiple   | 指定可以一次选择多个选项 |
| [name](./select_name.md)           | *name*     | 定义下拉列表的名称 |
| [required](./select_required.md)   | required   | 指定用户需要在提交表单之前选择一个值 |
| [size](./select_size.md)           | *number*   | 定义下拉列表中可见选项的数量 |

## 全局属性

`<select>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<select>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

将 \<select> 与 \<optgroup> 标签一起使用：

```html idoc:preview:iframe
<label for="cars">Choose a car:</label>
<select name="cars" id="cars">
  <optgroup label="Swedish Cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```
<!--rehype:style=height: 90px;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg