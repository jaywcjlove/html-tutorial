HTML onresize 事件属性
===

## 示例

调整浏览器窗口大小时执行 JavaScript：

```html idoc:preview:iframe
<body onresize="myFunction(this)">
  当前示例在iframe 中展示，无法调试：
  <span id="info"> </span>
  <script>
    function myFunction(evn) {
      document.getElementById('info').innerHTML = evn.innerHeight;
    }
  </script>
</body>
```

```html
<body onresize="myFunction()">
```

## 定义和使用

调整浏览器窗口大小时会触发 `onresize` 属性。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onresize | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onresize="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onresize 上运行的脚本 |
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

