HTML accesskey 属性
===

指定激活/聚焦元素的快捷键。

## 例子

具有指定访问键的两个超链接：

```html idoc:preview
<a href="https://www.w3schools.com/html/" accesskey="h">HTML</a><br>
<a href="https://www.w3schools.com/css/" accesskey="c">CSS</a>
```

## 定义和使用

`accesskey` 属性指定激活/聚焦元素的快捷键。

`accesskey` 属性值必须是单个字符（字母或数字）。


**警告** ⚠️

使用 `accesskeys` 很困难，因为它们可能与浏览器中的其他密钥标准冲突。
为了避免这个问题，大多数浏览器只有在同时按下 Alt 键时才会使用 `accesskeys`。

**关注点**

使访问密钥适应所有国际语言是很困难的。 `accesskey` 值可能不会出现在所有键盘上。 由于这些问题，建议不要使用访问 `accesskey`。


## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;accesskey&gt;__ | Yes | Yes | Yes | Yes | Yes |

## 语法

```HTML
<element accesskey="character">
```

## 属性值

值 Value | 描述 Description
---- | ----
character | 规定激活（使元素获得焦点）元素的便捷按键。

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg