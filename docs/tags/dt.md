HTML \<dt> Tag
===

## 示例

描述列表，包含术语和描述：

```html idoc:preview
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```

## 定义和用法

`<dt>` 标签在描述列表中定义了一个术语/名称。

`<dt>` 标记与 [\<dl>](./dl.md)（定义描述列表）和 [\<dd>](./dd.md)（描述每个术语/名称）结合使用。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<dt>   | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<dt>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<dt>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML Lists](../tutorial/lists.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<dt>` 元素：

```css
dt {
  display: block;
}
```