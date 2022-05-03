HTML \<menuitem> label 属性
===

## 示例

为不同的 \<menuitem> 元素指定标签：

```html idoc:preview:iframe
<menu type="context" id="mymenu">
  <menuitem label="Refresh"></menuitem>
  <menuitem label="Twitter"></menuitem>
  <menuitem label="Facebook"></menuitem>
</menu>
```

## 定义和用法

必需的标签属性指定命令/菜单项的名称，如向用户显示的那样。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| label | ❌ 不支持 | ❌ 不支持 | 8.0 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menuitem label="*text*">
```

## 属性值 Attribute Values

| 值 Value  | 描述 Description |
| ------ | ---- |
| *text* | 指定菜单项的可见标签 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg