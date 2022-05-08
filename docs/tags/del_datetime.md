HTML \<del> datetime 属性
===

## 示例

删除的文本，带有删除文本的日期和时间：

```html idoc:preview:iframe
<p>
  <del datetime="2015-11-15T22:55:03Z">此文字已被删除</del>
</p>
```

## 定义和用法

`datetime` 属性指定删除文本的日期和时间。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| datetime  | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

**注意：** `datetime` 属性在普通网络浏览器中没有视觉效果，但可以被屏幕阅读器使用。

## 语法

```html
<del datetime="YYYY-MM-DDThh:mm:ssTZD">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *YYYY-MM-DDThh:mm:ssTZD* | 删除文本的日期和时间。组件说明：<br>* YYYY - 年（例如 2012 年） <br>* MM - 月份（例如 01 表示一月） <br>* DD - 月份中的某天（例如 08） <br>* T 或空格 - 分隔符（如果还指定了时间，则需要） <br>* hh - 小时（例如 22 表示晚上 10 点） <br>* mm - 分钟（例如 55） <br>* ss - 秒（例如 03） <br>* TZD - 时区指示符（Z 表示祖鲁语，也称为格林威治标准时间） |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
