HTML onload 事件属性
===

## 示例

在页面加载后立即执行 JavaScript：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body onload="myFunction()">
  <h1>Hello World!</h1>
  <span id="info"> </span>
  <script>
    function myFunction() {
      document.getElementById('info').innerHTML = '页面已加载，执行了 onload 事件。';
    }
  </script>
</body>
</html>
```

```html
<body onload="myFunction()">
```

## 定义和使用

加载对象时会触发 `onload` 属性。

`onload` 最常用于 \<body> 元素中，用于在网页完全加载所有内容（包括图像、脚本文件、CSS 文件等）后执行脚本。 但是，它也可以用于其他元素（请参阅下面的“支持的 HTML 标记”）。

`onload` 属性可用于检查访问者的浏览器类型和浏览器版本，并根据这些信息加载适当版本的网页。

`onload` 属性也可用于处理 cookie（请参阅下面的“更多示例”）。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onload | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onload="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onload 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | \<body>, \<frame>, \<frameset>, \<iframe>, \<img>, \<input type="image">, \<link>, \<script> 和 \<style> |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

### 示例

在 \<img> 元素上使用 `onload`。 加载图像后立即提示“图像已加载”：

```html idoc:preview:iframe
<img src="../assets/chrome.svg" onload="loadImage()">
<div id="info"> </div>
<script>
  function loadImage() {
    document.getElementById('info').innerHTML = '图片已加载';
  }
</script>
```

### 示例

使用 `onload` 事件处理 `cookie`（使用“高级”javascript）：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body onload="checkCookies()">
  <p id="demo"></p>
  <script>
    function checkCookies() {
      var text = "";
      if (navigator.cookieEnabled == true) {
        text = "启用 Cookie。";
      } else {
        text = "未启用 Cookie。";
      }
      document.getElementById("demo").innerHTML = text;
    }
  </script>
</body>
</html>
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

