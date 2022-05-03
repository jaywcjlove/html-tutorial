HTML \<menuitem> checked 属性
===

## 示例

A pre-selected \<menuitem> element:

```html idoc:preview:iframe
<menu type="popup">
  <menuitem type="radio" radiogroup="alignment" checked
    label="Left" onclick="setAlign('left')">
</menu>
```

## 定义和用法

选中的属性是一个布尔属性。

如果存在，它指定在页面加载时应检查（预选） \<menuitem> 元素。

**注意：** 此属性只能在 type="checkbox" 或 type="radio" 时使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| checked   | ❌ 不支持 |❌ 不支持 |❌ 不支持 |❌ 不支持 |❌ 不支持 |

## 语法

```html
<menuitem checked>
```

[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg