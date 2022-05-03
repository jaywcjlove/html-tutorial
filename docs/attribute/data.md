HTML data 属性
===

## 定义和用法

`data` 属性指定对象要使用的资源的 URL。

## 适用于

`data` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<object>](../tags/object.md) | [data](../tags/object_data.md) |

## 示例

如何使用 \<object> 元素嵌入 Flash 文件：

```html idoc:preview:iframe
<object width="400" height="400" data="helloworld.swf"></object>
```

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| data      | Yes | Yes | Yes | Yes | Yes |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg