HTML onhashchange 事件属性
===

当 URL 的锚部分发生更改时运行的脚本

## 示例

当锚部分已更改时执行 JavaScript：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<body onhashchange="myFunction()">
  <p>单击按钮将当前 URL 的锚点部分更改为#part5</p>
  <button onclick="changePart()">Try it</button>
  <p id="demo"></p>
  <script>
  // 使用 location.hash 属性更改锚点部分
  function changePart() {
    location.hash = "part5";
    var x = "锚部分现在是：" + location.hash;
    document.getElementById("demo").innerHTML = x;
  }
  // 如果锚部分发生更改，则提醒一些文本
  function myFunction() {
    alert("锚部分变了！");
  }
  </script>
</body>
</html>
```

```html
<body onhashchange="myFunction()">
```

## 定义和使用

当当前 URL 的锚部分（以“#”符号开头）发生更改时，会触发 `onhashchange` 属性。

锚部分实际是什么的示例：假设当前 URL 是
`http://www.example.com/test.htm#part2` - 此 URL 的锚点部分将是 `#part2`。

要调用此事件，您可以：

* 通过设置 `Location Object` 的 `location.hash` 或 `location.href` 属性更改锚点部分
* 使用不同的书签导航到当前页面（使用“后退”或“前进”按钮）
*单击指向书签锚点的链接

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onhashchange    | 5.0  | 8.0 | 3.6 | 5.0 | 10.6 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onhashchange="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onhashchange 上运行的脚本 |
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


