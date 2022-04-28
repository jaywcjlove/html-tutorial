HTML \<b> 标签
===

## 示例

使一些文本加粗（不将其标记为重要）：


```html idoc:preview
<p>这是普通文本 - <b>这是粗体文本</b>。</p>
```

## 定义和用法

`<b>` 标签指定粗体文本，没有任何额外的重要性。

## 提示和注意事项

**注意：** 根据 HTML5 规范，当没有其他标签更合适时，应将 `<b>` 标签用作最后的手段。规范规定标题应使用 [\<h1> 到 \<h6>](./hn.md) 标签表示，强调文本应使用 [\<em>](./em.md) 标签表示，重要文本 应该用 [\<strong>](./strong.md) 标签表示，标记/突出显示的文本应该用 [\<mark>](./mark.md) 标签表示。

**提示：**您还可以使用以下 CSS 设置粗体文本：`font-weight: bold;`。

## 浏览器支持

| Element  | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<b>    | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<b>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<b>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例


使用 CSS 设置粗体文本：

```html idoc:preview
<p>这是普通文本 - <span style="font-weight:bold;">这是粗体文本</span>.</p>
```

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<b>` 元素：

```css
b {
  font-weight: bold;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg