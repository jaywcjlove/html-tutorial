HTML \<ul> 标签
===

## 示例

```html idoc:preview:iframe
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

## 定义和用法

`<ul>` 标签定义了一个无序（项目符号）列表。

使用 `<ul>` 标签和 [\<li>](./li.md) 标签来创建无序列表。

**提示：** 对于有序列表，请使用 [\<ol>](./ol.md) 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<ul>   | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<ul>` 标签支持 HTML 中的[全局属性](../reference/standardattribules.md)。

## 事件属性

`<ul>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

设置不同的列表样式类型（使用 CSS）：

```html idoc:preview:iframe
<ul style="list-style-type:circle">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
<ul style="list-style-type:disc">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
<ul style="list-style-type:square">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

扩展和减少列表中的行高（使用 CSS）：

```html idoc:preview:iframe
<ul style="line-height:180%">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<ul style="line-height:80%">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

在列表中创建一个列表（嵌套列表）：


```html idoc:preview:iframe
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```

创建一个更复杂的嵌套列表：


```html idoc:preview:iframe
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea
        <ul>
          <li>China</li>
          <li>Africa</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```

## 相关页面

HTML 教程: [HTML Lists](../tutorial/lists.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<ul>` 元素：

```css
ul {
  display: block;
  list-style-type: disc;
  margin-top: 1em;
  margin-bottom: 1 em;
  margin-left: 0;
  margin-right: 0;
  padding-left: 40px;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg