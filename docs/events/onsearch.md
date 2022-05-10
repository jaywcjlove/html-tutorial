HTML onsearch 事件属性
===

当用户在搜索字段中写入内容时触发 (`<input="search">`)

## 示例

提交搜索时执行 JavaScript：

```html idoc:preview:iframe
<p>在搜索字段中写一些东西，然后按“ENTER”。</p>
<input type="search" id="myInput" onsearch="myFunction()">
<p><strong>注意：</strong>Internet Explorer、Firefox 或 Opera 12 及更早版本不支持 onsearch 事件。</p>
<p id="demo"></p>
<script>
  function myFunction() {
    var x = document.getElementById("myInput");
    document.getElementById("demo").innerHTML = "您正在寻找：" + x.value;
  }
</script>
```

```html
<input type="search" onsearch="myFunction()">
```

## 定义和使用

`onsearch` 属性在用户按下 `ENTER` 键或单击类型为 `search` 的 [\<input>](../tags/input.md) 元素中的 `x` 按钮时触发。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onsearch | Yes | ❌ 不支持 | ❌ 不支持 | Yes | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onsearch="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 `onsearch` 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<input type="search">](../tags/input_type_search.md) |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


