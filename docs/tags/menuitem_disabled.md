HTML \<menuitem> disabled 属性
===

## 示例

禁用的 \<menuitem> 元素：

```html idoc:preview:iframe
<menu type="context" id="mymenu">
  <menuitem label="Refresh" icon="ico_reload.png" disabled></menuitem>
  <menuitem label="Twitter" icon="ico_twitter.png"></menuitem>
  <menuitem label="Facebook" icon="ico_facebook.png"></menuitem>
</menu>
```

## 定义和用法

disabled 属性是一个布尔属性。

如果存在，它指定应该禁用 \<menuitem> 元素。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| disabled  | ❌ 不支持 | ❌ 不支持 | 8.0 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menuitem disabled>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg