HTML \<textarea> Tag
===

## 示例

多行文本输入控件（文本区域）：

```html idoc:preview:iframe
<label for="review">评论：</label>
<br>
<textarea id="review" name="review" rows="4" cols="50">
在 HTML Tutorial，您将学习如何制作网站。 他们提供所有 Web 开发技术的免费教程。
</textarea>
```

## 定义和用法

`<textarea>` 标签定义了一个多行文本输入控件。

`<textarea>` 元素通常在表单中使用，以收集用户输入，如评论或评论。

一个文本区域可以容纳无限数量的字符，并且文本以固定宽度的字体（通常是 Courier）呈现。

文本区域的大小由 `<cols>` 和 `<rows>` 属性（或使用 CSS）指定。

表单提交后需要name属性引用表单数据（如果省略name属性，则不会提交文本区域的数据）。

需要 `id` 属性将文本区域与标签相关联。

**提示：** 始终添加 [\<label>](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<textarea> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [autofocus](./textarea_autofocus.md)     | autofocus          | 指定在页面加载时文本区域应自动获得焦点 |
| [cols](./textarea_cols.md)               | *number*           | 指定文本区域的可见宽度 |
| [dirname](./textarea_dirname.md)         | *textareaname*.dir | 指定将提交textarea的文本方向 |
| [disabled](./textarea_disabled.md)       | disabled           | 指定应禁用文本区域 |
| [form](./textarea_form.md)               | *form\_id*         | 指定文本区域属于哪个表单 |
| [maxlength](./textarea_maxlength.md)     | *number*           | 指定文本区域中允许的最大字符数 |
| [name](./textarea_name.md)               | *text*             | 指定文本区域的名称 |
| [placeholder](./textarea_placeholder.md) | *text*             | 指定描述文本区域预期值的简短提示 |
| [readonly](./textarea_readonly.md)       | readonly           | 指定文本区域应该是只读的 |
| [required](./textarea_required.md)       | required           | 指定需要/必须填写文本区域 |
| [rows](./textarea_rows.md)               | *number*           | 指定文本区域中可见的行数 |
| [wrap](./textarea_wrap.md)               | hard soft          | 指定在表单中提交时如何包装文本区域中的文本 |

## 全局属性

`<textarea>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<textarea>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例


禁用默认调整大小选项：

```html idoc:preview:iframe
<style>
  textarea { resize: none; }
</style>
<label for="review">评论：</label>
<br>
<textarea id="review" name="review" rows="4" cols="50">
在 HTML Tutorial，您将学习如何制作网站。 他们提供所有 Web 开发技术的免费教程。
</textarea>
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg