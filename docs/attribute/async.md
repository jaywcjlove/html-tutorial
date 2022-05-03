HTML async 属性
===

## 定义和用法

`async` 属性是一个布尔属性。

如果存在，它指定脚本将在可用时立即异步执行。

**注意：** `async` 属性仅适用于外部脚本（并且仅应在存在 `src` 属性时使用）。

**注意：** 有几种方法可以执行外部脚本：

* 如果 `async` 存在：脚本与页面的其余部分异步执行（脚本将在页面继续解析时执行）
* 如果 `async` 不存在且 [`defer`](../tags/script_defer.md) 存在：脚本在页面完成解析后执行
* 如果 `async` 或 [`defer`](../tags/script_defer.md) 都不存在：在浏览器继续解析页面之前立即获取并执行脚本

## 适用于

`async` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<script>](../tags/script.md) | [async](../tags/script_async.md) |

## Script 示例

一个将在可用时立即异步运行的脚本：

```html
<script src="demo_async.js" async></script>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| async     | Yes | 10.0 | 3.6 | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg