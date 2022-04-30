HTML \<input type="search">
===

## 示例

定义搜索字段（如站点搜索或 Google 搜索）：

```html idoc:preview:iframe
<label for="gsearch">Search Google:</label>
<input type="search" id="gsearch" name="gsearch">
```

## 定义和用法

`<input type="search">` 定义了一个用于输入搜索字符串的文本字段。

**注意：** 记得给搜索字段设置一个名字，否则什么都不会提交。 搜索输入最常用的名称是 q。

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="search" | 26.0 | 10.0 | 4.0 | 5.1 | 12.1 |

## 语法

```html
<input type="search">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg