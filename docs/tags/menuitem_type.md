HTML \<menuitem> type 属性
===

## 示例

A \<menuitem> element of type "command":

```html
<menu>
  <menuitem type="command" label="Save" onclick="save()">Save</menuitem>
</menu>
```

## 定义和用法

type 属性指定命令/菜单项的类型。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type      | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menuitem type="command|checkbox|radio">
```

## 属性值 Attribute Values

| 值 Value  | 描述 Description |
| ------ | ---- |
| command  | Default. Specifies a normal command with an action           |
| checkbox | Specifies a command that can be toggled using a checkbox     |
| radio    | Specifies a command that can be toggled using a radio button |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg