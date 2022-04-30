HTML \<menuitem> radiogroup 属性
===

## 示例

属于无线电组的 \<menuitem> 元素：

```html idoc:preview:iframe
<menu>
  <menuitem type="radio" label="Left" radiogroup="alignment" onclick="setAlign('left')">Left</menuitem>
</menu>
```

## 定义和用法

radiogroup 属性指定命令/菜单项本身被激活/切换时将被切换的命令组的名称。

**注意：** 此属性只能在 type="radio" 时使用。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| radiogroup | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menuitem radiogroup="*groupname*">
```

## 属性值 Attribute Values

| 值 Value  | 描述 Description |
| ------ | ---- |
| *groupname* | 指定当命令本身被激活/切换时将被切换的命令组的名称（仅适用于 type="radio"） |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg