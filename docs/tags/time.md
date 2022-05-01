HTML \<time> Tag
===

## 示例

如何定义时间和日期：

```html idoc:preview:iframe
<p>每个工作日的开放时间为 <time>10:00</time> 至 <time>21:00</time>。</p>

<p>我在<time datetime="2008-02-14 20:00">情人节</time>有个约会。</p>
```

## 定义和用法

`<time>` 标签定义了一个特定的时间（或日期时间）。

该元素的 `datetime` 属性用于将时间转换为机器可读的格式，以便浏览器可以通过用户的日历提供添加日期提醒，并且搜索引擎可以产生更智能的搜索结果。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<time> | 62.0 | 18.0 | 22.0 | 7.0 | 49.0 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [datetime](./time_datetime.md) | *datetime* | 表示 \<time> 元素的机器可读格式 |

## 全局属性

`<time>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<time>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg