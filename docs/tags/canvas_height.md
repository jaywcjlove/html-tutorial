HTML \<canvas> height 属性
===

## 示例

一个高度和宽度为 `200` 像素的 \<canvas> 元素：

```html idoc:preview:iframe
<canvas
  id="myCanvas"
  width="200"
  height="200"
  style="border:1px solid"
>
```

## 定义和用法

`height` 属性指定 `<canvas>` 元素的高度，以像素为单位。

**提示：** 使用 `width` 属性指定 `<canvas>` 元素的宽度，以像素为单位。

**提示：** 每次重新设置画布的高度或宽度时，画布内容都会被清除（参见页面底部的示例）。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| height    | 4.0 | 9.0 | 2.0 | 3.1 | 9.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<canvas height="pixels">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *pixels* | 指定画布的高度，以像素为单位（例如“100”）。 默认值为 150 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

通过设置宽度或高度属性（使用 JavaScript）清除画布：

```html idoc:preview:iframe
<canvas id="myCanvas" width="200" height="200" style="border:1px solid"></canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "#92B901";
  ctx.fillRect(50, 50, 100, 100);
  function clearCanvas() {
      c.height = 300;
  }
</script>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
