HTML ontoggle 事件属性
===

## 示例

当 \<details> 元素打开或关闭时执行 JavaScript：

```html
<details ontoggle="myFunction()">
```

```html idoc:preview:iframe
<details ontoggle="myFunction()">
<summary>HyperText Markup Language</summary>
<p>HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。</p>
</details>
<script>
  function myFunction() {
    alert("The ontoggle event occured");
  }
</script>
```

## 定义和使用

当用户打开或关闭 [\<details>](../tags/details.md) 元素时，会触发 toggle 属性。

[\<details>](../tags/details.md) 元素指定用户可以按需查看或隐藏的其他详细信息。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| ontoggle | 12.0  | 79.0 | 48.0  | 6.0 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element ontoggle="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 在 toggle 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<details>](../tags/details.md) |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg


