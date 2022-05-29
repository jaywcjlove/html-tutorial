HTML `spellcheck` 属性
===

是否要检查元素的拼写和语法。

## 实例

带有拼写检查的可编辑段落：

```html idoc:preview
<p contenteditable="true" spellcheck="true">这是一个段落，不检查英文单词拼写。</p>
<input spellcheck="false" placeholder="不检查英文单词拼写">
<input spellcheck="true" placeholder="检查英文单词拼写">
```

## 定义和使用

`spellcheck` 属性指定是否要检查元素的拼写和语法。

可以对以下内容进行拼写检查：

- `<input>`元素中的文本值（不是密码）
- `<textarea>` 元素中的文本
- 可编辑元素中的文本

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;spellcheck&gt;__ | 9.0 | 10.0 | 2.0 | 5.1 | 10.5 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element spellcheck="true|false">
```

## 属性值

值 Value | 描述 Description
---- | ----
true | 该元素将检查其拼写和语法
false | 不检查元素

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg