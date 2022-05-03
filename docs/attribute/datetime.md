HTML datetime 属性
===

## 定义和用法

`datetime` 属性指定删除/插入文本的日期和时间。

当与 `<time>` 元素一起使用时，它表示 `<time>` 元素的日期和/或时间。

## 适用于

`datetime` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<del>](../tags/del.md)   | [datetime](../tags/del_datetime.md)  |
| [\<ins>](../tags/ins.md)   | [datetime](../tags/ins_datetime.md)  |
| [\<time>](../tags/time.md) | [datetime](../tags/time_datetime.md) |

## 示例

### Del 示例

删除的文本，带有删除文本的日期和时间：

```html idoc:preview:iframe
<p>
  <del datetime="2015-11-15T22:55:03Z">此文字已被删除</del>
</p>
```

### Ins 示例

插入的文本，带有插入文本的日期和时间：

```html idoc:preview:iframe
<p>
  这是一个文本。
  <ins datetime="2015-09-15T22:55:03Z">这是插入的文本。</ins>
</p>
```

### Time 示例

具有机器可读日期时间属性的时间元素：

```html idoc:preview:iframe
<p>我在 <time datetime="2017-02-14">情人节</time>有个约会。</p>
```

## 浏览器支持

`datetime` 属性对每个元素都有以下浏览器支持：

| 元素 Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| [del](../tags/del.md)     | Yes | Yes | Yes | Yes | Yes |
| [ins](../tags/ins.md)     | Yes | Yes | Yes | Yes | Yes |
| [time](../tags/time.md)    | Yes | Yes | Yes | Yes | Yes |


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
