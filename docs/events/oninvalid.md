HTML oninvalid 事件属性
===

元素无效时运行的脚本

## 示例

当输入字段无效时执行 JavaScript：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  名字: <input type="text" oninvalid="alert('您必须填写表格！');" name="fname" required>
  <input type="submit" value="Submit">
</form>
<p>如果您单击提交，而不填写文本字段，则会出现警告消息。</p>
<p><strong>注意：</strong> Safari 不支持 oninvalid 事件。</p>
```

```html
<input type="text" oninvalid="alert('您必须填写表格！');" required>
```

## 定义和使用

当可提交的 [\<input>](../tags/input.md) 元素无效时，会发生 oninvalid 事件。

例如，如果设置了 required 属性并且该字段为空，则输入字段无效（required属性指定必须在提交表单之前填写输入字段）。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| oninvalid       | Yes | 10.0 | Yes | ❌ 不支持 | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element oninvalid="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 oninvalid 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<input>](../tags/input.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

当输入字段无效时执行 JavaScript：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  名字: <input type="text" oninvalid="alert('必须包含 6 个或更多字符');" name="fname" pattern=".{6,}">
  <input type="submit" value="Submit">
</form>
如果您提交的输入字段少于 6 个字符，则会出现警告消息。
<br>
<strong>注意：</strong> Safari 不支持 oninvalid 事件。
```

```html
<input type="text" oninvalid="alert('必须包含 6 个或更多字符');" pattern=".{6,}">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

