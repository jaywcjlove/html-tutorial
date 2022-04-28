HTML data-* 属性
===

用于存储页面或应用程序私有的自定义数据。

## 实例

使用 data-* 属性来嵌入自定义数据：

```html idoc:preview
<ul>
  <li data-animal-type="鸟类">喜鹊</li>
  <li data-animal-type="鱼类">金枪鱼</li> 
  <li data-animal-type="蜘蛛">蝇虎</li> 
</ul>
```

## 定义和使用

`data-*` 属性用于存储页面或应用程序私有的自定义数据。

`data-*` 属性使我们能够在所有 HTML 元素上嵌入自定义数据属性。

然后可以在页面的 JavaScript 中使用存储的（自定义）数据来创建更具吸引力的用户体验（无需任何 Ajax 调用或服务器端数据库查询）。

`data-*` 属性由两部分组成：

1. 属性名称不能包含任何大写字母，并且必须在前缀 `data-` 之后至少有一个字符长
2. 属性值可以是任何字符串

⚠️ 注意：以 `data-` 为前缀的自定义属性将被用户代理完全忽略。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;data-*&gt;__ | 4.0 | 5.5 | 2.0 | 3.1 | 9.6 |

## 语法

```html
<element data-*="somevalue">
```

## 属性值

值 Value | 描述 Description
---- | ----
somevalue | 指定属性的值（作为字符串）


[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg