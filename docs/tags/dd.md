HTML \<dd> Tag
===

## 示例

描述列表，包含术语和描述：

```html idoc:preview:iframe
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```

## 定义和用法

`<dd>` 标签用于描述描述列表中的术语/名称。

`<dd>` 标记与 [\<dl>](./dl.md)（定义描述列表）和 [\<dt>](./dt.md)（定义术语/名称）结合使用。

在 `<dd>` 标记内，您可以放置段落、换行符、图像、链接、列表等。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --------- | --- | --- | --- | --- | --- |
| \<dd>   | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<dd>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<dd>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<dd>` 元素：

```css
dd {
  display: block;
  margin-left: 40px;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg