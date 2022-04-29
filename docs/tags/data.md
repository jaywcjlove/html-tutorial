HTML \<data> 标签
===

## 示例

以下示例显示产品名称，但还将每个名称与产品编号相关联：

```html idoc:preview
<ul>
  <li><data value="21053">Cherry Tomato</data></li>
  <li><data value="21054">Beef Tomato</data></li>
  <li><data value="21055">Snack Tomato</data></li>
</ul>
```

## 定义和用法

`<data>` 标签用于添加给定内容的机器可读翻译。

该元素既为数据处理器提供机器可读值，又为在浏览器中呈现的人类可读值提供。

**提示：** 如果内容与时间或日期相关，请改用 [\<time>](./time.md) 元素。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<data> | 62.0 | 13.0 | 22.0 | Not supported | 49.0 |

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ---- | ---- | ---- |
| value | *machine-readable format* | 指定元素内容的机器可读翻译 |

## 全局属性

`<data>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg