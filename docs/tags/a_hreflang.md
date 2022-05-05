HTML `<a>` 标签的 hreflang 属性
===

## 示例

`hreflang` 属性指定链接中文档的语言：

```html idoc:preview
<a target="_blank" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

## 定义和用法

`hreflang` 属性指定链接文档的语言。

此属性仅在设置了 `href` 属性时使用。

**注意：** 此属性仅供参考。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| hreflang  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<a hreflang="language_code">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| *language\_code* | 一个由两个字母组成的语言代码，用于指定链接文档的语言。 要查看所有可用的语言代码，请访问我们的 [语言代码参考](../reference/language_codes.md)。 |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg