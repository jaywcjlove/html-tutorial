HTML onpageshow 事件属性
===

当用户导航到页面时运行的脚本

## 示例

当用户导航到网页时执行 JavaScript：

```html idoc:preview:iframe
<body onpageshow="myFunction()">
  <h1>Hello World!</h1>
  页面执行 onpageshow 事件：<span id="info"> </span>
  <script>
    function myFunction() {
      document.getElementById('info').innerHTML = 'Welcome!';
    }
  </script>
</body>
```

```html
<body onpageshow="myFunction()">
```

## 定义和使用

`onpageshow` 事件在用户导航到网页时发生。

`onpageshow` 事件类似于 [onload](./onload.md) 事件，只是它在页面首次加载时发生在 `onload` 事件之后。 此外，每次加载页面时都会发生 `onpageshow` 事件，而从缓存加载页面时不会发生 `onload` 事件。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onpageshow      | Yes | 11.0 | Yes | 5.0 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onpageshow="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onpageshow 上运行的脚本 |
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

