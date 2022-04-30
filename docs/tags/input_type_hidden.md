HTML \<input type="hidden">
===

## 示例

定义一个隐藏字段：

```html idoc:preview:iframe
<input type="hidden" id="custId" name="custId" value="3487">
```

## 定义和用法

`<input type="hidden">` 定义了一个隐藏的输入字段。

一个隐藏字段允许 Web 开发人员在提交表单时包含用户无法看到或修改的数据。

隐藏字段通常存储提交表单时需要更新的数据库记录。

**注意：** 虽然该值不会在页面内容中向用户显示，但可以使用任何浏览器的开发人员工具或“查看源代码”功能看到（并且可以编辑）。 不要使用隐藏输入作为一种安全形式！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="hidden" | 1.0 | Yes | 1.0 | 1.0 | 1.0 |

## 语法

```html
<input type="hidden">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg