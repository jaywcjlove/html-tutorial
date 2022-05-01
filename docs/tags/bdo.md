HTML \<bdo> 标签
===

## 示例

指定文本方向：

```html idoc:preview
<bdo dir="rtl">
This text will go right-to-left.
</bdo>
```

## 定义和用法

BDO 表示双向超控(Bi-Directional Override)。

`<bdo>` 标签用于覆盖当前文本方向。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<bdo>  | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 Attribute | 值 Value | 描述 Description |
| ----- | ----- | ----- |
| [dir](./bdo_dir.md) | `ltr` `rtl` | 必需的。 指定 `<bdo>` 元素内文本的文本方向 |


## 全局属性

`<bdo>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<bdo>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<bdo>` 元素：

```css
bdo {
  unicode-bidi: bidi-override;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg