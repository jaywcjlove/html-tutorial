HTML \<script> Tag
===

## 示例

写“你好 JavaScript！” 使用 JavaScript：

```html idoc:preview:iframe
<div id="demo"></div>
<script>
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```

## 定义和用法

`<script>` 标签用于嵌入客户端脚本 (JavaScript)。

`<script>` 元素要么包含脚本语句，要么通过 [src](./script_src.md) 属性指向外部脚本文件。

JavaScript 的常见用途是图像处理、表单验证和内容的动态更改。

## 提示和注意事项

**提示：** 对于在浏览器中禁用脚本或浏览器不支持客户端脚本的用户，还请查看 [\<noscript>](./noscript.md) 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<script> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [async](./script_async.md) | async | 指定脚本与解析页面并行下载，并在它可用时立即执行（在解析完成之前）（仅适用于外部脚本） |
| [crossorigin](./script_crossorigin.md) | anonymous<br>use-credentials | 将请求的模式设置为 HTTP CORS 请求 |
| [defer](./script_defer.md) | defer | 指定与解析页面并行下载脚本，并在页面解析完成后执行（仅适用于外部脚本） |
| [integrity](./script_integrity.md) | *filehash* | 允许浏览器检查获取的脚本，以确保如果源已被操纵，则永远不会加载代码 |
| nomodule | True<br>False | 指定脚本不应在支持 ES2015 模块的浏览器中执行 |
| [referrerpolicy](./script_referrepolicy.md) | no-referrer<br>no-referrer-when-downgrade<br>origin<br>origin-when-cross-origin<br>same-origin<br>strict-origin<br>strict-origin-when-cross-origin<br>unsafe-url | 指定在获取脚本时要发送的引荐来源信息 |
| [src](./script_src.md) | *URL* | 指定外部脚本文件的 URL |
| [type](./script_type.md) | *scripttype* | 指定脚本的媒体类型 |

## HTML 和 XHTML 之间的区别

在 XHTML 中，脚本中的内容被声明为 _#PCDATA_ (而不是 _CDATA_)，这意味着实体将被解析。

这意味着在 XHTML 中，所有特殊字符都应该被编码，或者所有内容都应该包含在 _CDATA_ 部分中：

```html
<script type="text/javascript">
//<![CDATA[
var i = 10;
if (i < 5) {
  // some code
}
//]]>
</script>
```

## 全局属性

`<script>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 相关页面

HTML 教程: [HTML Scripts](../tutorial/scripts.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<script>` 元素：

```css
script {
  display: none;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg