HTML \<menuitem> Tag
===

[![](https://shields.io/badge/HTML5-已弃用/过时-yellow?logo=HTML5)](https://caniuse.com/?search=<menuitem>)

## 示例

具有不同 \<menuitem> 元素的上下文菜单：

```html idoc:preview:iframe
<menu type="context" id="mymenu">
  <menuitem label="Refresh" onclick="window.location.reload();" icon="ico_reload.png">
  </menuitem>
  <menu label="Share on...">
    <menuitem label="Twitter" icon="ico_twitter.png"
    onclick="window.open('//twitter.com/intent/tweet?text='+window.location.href);">
    </menuitem>
    <menuitem label="Facebook" icon="ico_facebook.png"
    onclick="window.open('//facebook.com/sharer/sharer.php?u='+window.location.href);">
    </menuitem>
  </menu>
  <menuitem label="Email This Page"
  onclick="window.location='mailto:?body='+window.location.href;"></menuitem>
</menu>
```

## 定义和用法

\<menuitem> 标签在 HTML5 中已弃用。

\<menuitem> 标记定义用户可以从弹出菜单调用的命令/菜单项。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<menuitem> | ❌ 不支持 | ❌ 不支持 | 8.0 (for context menus) | ❌ 不支持 | ❌ 不支持 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [checked](./menuitem_checked.md)       | checked | 指定在页面加载时应检查命令/菜单项。 仅适用于 type="radio" 或 type="checkbox" |
| command                                   |   |   |
| [default](./menuitem_default.md)       | default | 将命令/菜单项标记为默认命令 |
| [disabled](./menuitem_disabled.md)     | disabled | 指定应禁用命令/菜单项 |
| [icon](./menuitem_icon.md)             | *URL* | 指定命令/菜单项的图标 |
| [label](./menuitem_label.md)           | *text* | Required. 指定命令/菜单项的名称，向用户显示 |
| [radiogroup](./menuitem_radiogroup.md) | *groupname* | 指定当命令/菜单项本身被切换时将被切换的命令组的名称。 仅适用于 type="radio" |
| [type](./menuitem_type.md)             | checkbox <br> command <br> radio | 指定命令/菜单项的类型。 默认为“命令” |

## 全局属性

`<menuitem>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<menuitem>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
