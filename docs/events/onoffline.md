HTML onoffline 事件属性
===

浏览器开始离线工作时运行的脚本

## 示例

当浏览器开始离线工作时执行 JavaScript：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body ononline="onFunction()" onoffline="offFunction()">
  <p>打开“文件”菜单并单击“离线工作”以在在线和离线工作之间切换.</p>
  <script>
  function onFunction() {
    alert ("您的浏览器正在联机工作。");
  }
  function offFunction() {
    alert ("您的浏览器正在离线工作。");
  }
  </script>
</body>
</html>
```

```html
<body onoffline="myFunction()">
```

## 定义和使用

`onoffline` 属性在浏览器开始离线工作时触发。

**提示：** `onoffline` 属性与 [ononline](./ononline.md) 属性相反。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onoffline | 3 | 12 | 9 | 4 | 15 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onoffline="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onoffline 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | \<body> |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

