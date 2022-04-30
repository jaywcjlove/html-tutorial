HTML \<menu> label 属性
===

## 示例

标签属性的使用：

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

label 属性指定菜单的可见标签。

label 属性通常用于标记菜单中的嵌套菜单。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| label | ❌ 不支持 | ❌ 不支持 | 8.0 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<menu label="*text*">
```

## 属性值 Attribute Values

| 值 Value  | 描述 Description |
| ------ | ---- |
| *text* | 指定菜单的可见标签 |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg