HTML \<dialog> open 属性
===

## 示例

使用 \<dialog> 元素：

```html idoc:preview:iframe
<dialog open>
  这是一个打开的对话窗口
</dialog>
```

⚠️ 默认不支持，但可以在 `about:config` 中启用（设置 `dom.dialog_element.enabled` 为 true）。

## 定义和用法

`open` 属性是一个布尔属性。

当存在时，它指定对话框元素处于活动状态并且用户可以与之交互。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| open      | 37.0 | 79.0 | 53.0\* | Not supported | 24.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

⚠️ 默认不支持，但可以在 `about:config` 中启用（设置 `dom.dialog_element.enabled` 为 true）。

## 语法

```html
<dialog open>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
