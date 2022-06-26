HTML oncontextmenu 属性
===

## 定义和用法

`oncontextmenu` 属性在用户右键单击元素以打开上下文菜单时触发。

**注意：** 虽然所有浏览器都支持 `oncontextmenu` 事件，但目前只有 Firefox 支持 `contextmenu` 属性。

## 适用于

`oncontextmenu` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [oncontextmenu](../events/oncontextmenu.md) |

### 示例

触发上下文菜单时执行 JavaScript：


```html
<div oncontextmenu="myFunction()" contextmenu="mymenu">
```

```html idoc:preview:iframe
<style>
  div {
    background: yellow;
    border: 1px solid black;
    padding: 10px;
  }
</style>
<div oncontextmenu="myFunction()" contextmenu="mymenu">
<p>在此框内右键单击以查看上下文菜单！</p>

<menu type="context" id="mymenu">
  <menuitem label="Refresh" onclick="window.location.reload();" icon="ico_reload.png"></menuitem>
  <menu label="Share on...">
    <menuitem label="Twitter" icon="ico_twitter.png" onclick="window.open('//twitter.com/intent/tweet?text=' + window.location.href);"></menuitem>
    <menuitem label="Facebook" icon="ico_facebook.png" onclick="window.open('//facebook.com/sharer/sharer.php?u=' + window.location.href);"></menuitem>
  </menu>
  <menuitem label="Email This Page" onclick="window.location='mailto:?body='+window.location.href;"></menuitem>
</menu>

</div>

<p><strong>注意：</strong> contextmenu <strong>属性</strong>仅适用于 Firefox！ </p>

<script>
function myFunction() {
  alert("You right-clicked inside the div!");
}
</script>
```

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oncontextmenu   | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg



