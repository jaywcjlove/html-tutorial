HTML \<dir> 标签
===

[![](https://shields.io/badge/HTML5-已弃用/过时-yellow?logo=HTML5)](https://caniuse.com/?search=<dir>)

## 示例

```html idoc:preview:iframe
<dir>
  <li>HTML</li>
  <li>XHTML</li>
  <li>CSS</li>
</dir>
```

## HTML5 不支持

`<dir>` 标签在 HTML 4 中用于列出目录标题。

## 改用什么？

使用 [\<ul>](./ul.md) 创建目录列表：

```html idoc:preview:iframe
<ul>
  <li>html</li>
  <li>xhtml</li>
  <li>css</li>
</ul> 
```

减少列表中的行高（使用 CSS）：

```html idoc:preview:iframe
<ul style="line-height:80%">
  <li>html</li>
  <li>xhtml</li>
  <li>css</li>
</ul>
```