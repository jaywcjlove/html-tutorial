HTML \<dialog> 标签
===

## 示例

使用 \<dialog> 元素：

```html idoc:preview:iframe
<dialog open>This is an open dialog window</dialog>
```
<!--rehype:style=min-height: 110px;-->

## 定义和用法

`<dialog>` 标签定义了一个对话框或子窗口。

`<dialog>` 元素使在网页上创建弹出对话框和模式变得容易。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<dialog> | 37.0 | 79.0 | 53.0\* | ❌ 不支持 | 24.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

\* 默认不支持，但可以在 `about:config` 中启用（设置 `dom.dialog_element.enabled` 为 `true`）。

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| [open](./dialog_open.md) | open  | 指定对话框元素处于活动状态并且用户可以与之交互 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 全局属性

`<dialog>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<dialog>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg