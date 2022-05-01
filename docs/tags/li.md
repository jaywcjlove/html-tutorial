HTML \<li> 标签
===

## 示例

一个有序 ([\<ol>](./ol.md)) 和一个无序 ([\<ul>](./ul.md)) HTML 列表：

```html idoc:preview:iframe
<ol>
  <li>咖啡</li>
  <li>茶</li>
  <li>牛奶</li>
</ol>

<ul>
  <li>咖啡</li>
  <li>茶</li>
  <li>牛奶</li>
</ul>
```

## 定义和用法

`<li>` 标签定义了一个列表项。

`<li>` 标签用于有序列表 ([\<ol>](./ol.md))、无序列表 ([\<ul>](./ul.md)) 和菜单列表 ([\<menu>](./menu.md))。

在 [\<ul>](./ul.md) 和 [\<menu>](./menu.md) 中，列表项通常会以项目符号显示。

在 \<ol> 中，列表项通常以数字或字母显示。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<li>   | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [value](./li_value.md) | *number* | 仅适用于 \<ol> 列表。 指定列表项的起始值。 以下列表项将从该数字递增 |

## 全局属性

`<li>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<li>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

在有序列表中使用 value 属性：

```html idoc:preview:iframe
<ol>
  <li value="100">Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
  <li>Water</li>
  <li>Juice</li>
  <li>Beer</li>
</ol>
```

设置不同的列表样式类型（使用 CSS）：

```html idoc:preview:iframe
<ol>
  <li>Coffee</li>
  <li style="list-style-type:lower-alpha">Tea</li>
  <li>Milk</li>
</ol>

<ul>
  <li>Coffee</li>
  <li style="list-style-type:square">Tea</li>
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

HTML 教程: [HTML Lists](../tutorial/links.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<li>` 元素：

```css
li {
  display: list-item;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg