HTML data-\* 属性
===

## 定义和用法

`data-*` 属性用于存储页面或应用程序私有的自定义数据。

`data-*` 属性使我们能够在所有 HTML 元素上嵌入自定义数据属性。

然后可以在页面的 JavaScript 中使用存储的（自定义）数据来创建更具吸引力的用户体验（无需任何 Ajax 调用或服务器端数据库查询）。

`data-*` 属性由两部分组成：

1. 属性名不能包含任何大写字母，并且必须在前缀 “data-” 之后至少有一个字符长
2. 属性值可以是任意字符串

**注意：** 以 “data-” 为前缀的自定义属性将被用户代理完全忽略。

## 适用于

`data-*` 属性是一个 [全局属性](../reference/standardattributes.md)，可用于任何 HTML 元素。

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| 全部 [HTML](../reference/byfunc.md) 元素 | [data-\*](./global/data.md) |

## 示例

使用 `data-\*` 属性嵌入自定义数据：

```html idoc:preview:iframe
<ul>
  <li data-animal-type="bird">Owl</li>
  <li data-animal-type="fish">Salmon</li>
  <li data-animal-type="spider">Tarantula</li>
</ul>
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| data-\*   | 4.0 | 5.5 | 2.0 | 3.1 | 9.6 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg