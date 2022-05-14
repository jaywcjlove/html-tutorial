HTML \<menu> Tag
===

[![](https://shields.io/badge/HTML5-实验性标签-green?logo=HTML5)](https://caniuse.com/?search=<menu>)

## 示例

具有不同 \<menuitem> 元素的上下文菜单：

```html idoc:preview:iframe
<menu type="context" id="mymenu">
  <menuitem label="Refresh" onclick="window.location.reload();" icon="ico_reload.png">
  </menuitem>
  <menu label="Share on...">
    <menuitem label="Twitter" icon="../assets/opera.svg"
    onclick="window.open('//twitter.com/intent/tweet?text='+window.location.href);">
    </menuitem>
    <menuitem label="Facebook" icon="../assets/chrome.svg"
    onclick="window.open('//facebook.com/sharer/sharer.php?u='+window.location.href);">
    </menuitem>
  </menu>
  <menuitem label="Email This Page"
  onclick="window.location='mailto:?body='+window.location.href;"></menuitem>
</menu>
```

## 定义和用法

\<menu> 标签定义命令列表/菜单。

\<menu> 标签用于上下文菜单、工具栏以及用于列出表单控件和命令。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<menu> | ❌ 不支持 | ❌ 不支持 | 8.0 (only context menus) | ❌ 不支持 | ❌ 不支持 |

**注意：** \<menu> 标签仅在 Firefox 中受支持，并且仅适用于上下文菜单。

## 提示和注意事项

**提示：** 使用 CSS 设置菜单列表的样式。

**警告：** ⚠️ 此功能是实验性的。 在生产中使用之前要小心。

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [label](./menu_label.md) | *text* | 指定菜单的可见标签 |
| [type](./menu_type.md)   | list<br>toolbar<br>context | 指定要显示的菜单类型 |

## 全局属性

`<menu>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<menu>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<menu>` 元素：

```css
menu {
  display: block;
  list-style-type: disc;
  margin-top: 1em;
  margin-bottom: 1em;
  margin-left: 0;
  margin-right: 0;
  padding-left: 40px;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg