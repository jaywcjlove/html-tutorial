HTML \<menu> type 属性
===

## 示例

上下文菜单：

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

type 属性指定菜单的类型。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type      | ❌ 不支持 | ❌ 不支持 | 8.0 (only type="context") | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menu type="list|context|toolbar">
```


## 属性值 Attribute Values

| 值 Value  | 描述 Description |
| ------ | ---- |
| list    | 默认。指定一个列表菜单。 用户可以执行或激活的命令列表（li 元素） |
| context | 指定上下文菜单。 必须先激活菜单，然后用户才能与命令交互 |
| toolbar | 指定工具栏菜单。 活动命令，允许用户立即与命令交互 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
