HTML accesskey 属性
===

## 定义和用法

`accesskey` 属性指定激活/聚焦元素的快捷键。

**注意：** 不同浏览器访问快捷键的方式不同：

| 浏览器 | Windows | Linux | Mac |
| ----- | ----- | ----- | ----- |
| Internet Explorer | \[Alt] + *accesskey* | N/A | |
| Chrome            | \[Alt] + *accesskey* | \[Alt] + *accesskey* | \[Control] \[Alt] + *accesskey* |
| Firefox           | \[Alt] \[Shift] + *accesskey* | \[Alt] \[Shift] + *accesskey* | \[Control] \[Alt] + *accesskey* |
| Safari            | \[Alt] + *accesskey* | N/A                           | \[Control] \[Alt] + *accesskey* |
| Opera             | Opera 15 或更高版本: \[Alt] + *accesskey* <br>Opera 12.1 或更高版本: \[Shift] \[Esc] + *accesskey* | | |
<!--rehype:style=width: 100%; display: inline-table;-->

但是，在大多数浏览器中，快捷方式可以设置为另一种组合键。

**提示：** 如果多个元素具有相同的访问密钥，则行为不同：

* IE、Firefox：按下访问键的下一个元素将被激活
* Chrome、Safari：按下访问键的最后一个元素将被激活
* Opera：按下访问键的第一个元素将被激活

## 适用于

`accesskey` 是 [全局属性](../reference/standardattributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 全部 [HTML](../tags/README.md) 元素 | [accesskey](./global/accesskey.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

### 示例

具有指定访问键的两个超链接：

```html idoc:preview:iframe
<a href="https://github.com/jaywcjlove/html-tutorial" accesskey="h">HTML5</a><br>
<a href="https://github.com/jaywcjlove/c-tutorial" accesskey="c">C 语言</a>
```

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| accesskey | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg