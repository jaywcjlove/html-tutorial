HTML \<input type="button">
===

## 示例

单击时激活 JavaScript 的按钮：

```html idoc:preview:iframe
<script>
  function msg() {
    alert("Hello world!");
  }
</script>
<input type="button" value="Click me" onclick="msg()">
```

## 定义和用法

`<input type="button">` 定义了一个可点击的按钮（主要与 JavaScript 一起使用来激活脚本）。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="button" | 1.0 | Yes | 1.0 | 1.0 | Yes |

## 语法

```html
<input type="button">
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg