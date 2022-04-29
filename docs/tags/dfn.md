HTML \<dfn> Tag
===

## 示例

用 \<dfn> 标记一个术语：

```html idoc:preview:iframe
<p><dfn>HTML</dfn> 是创建网页的标准标记语言。</p>
```

## 定义和用法

`<dfn>` 标签代表“定义元素”，它指定将在内容中定义的术语。

`<dfn>` 标记的最近父项还必须包含该术语的定义/解释。

`<dfn>` 标记内的术语可以是以下任何一种：

**1. 就像 **`<dfn>`** 元素的内容：**


```html idoc:preview:iframe
<p><dfn>HTML</dfn> 是创建网页的标准标记语言。</p>
```

**2. 或者，添加了 title 属性：**


```html idoc:preview:iframe
<p><dfn title="HyperText Markup Language">HTML</dfn> 是创建网页的标准标记语言。</p>
```

**3. 或者，在 **`<dfn>`** 元素中使用 \<abbr> 标记：**


```html idoc:preview
<p><dfn><abbr title="HyperText Markup Language">HTML</abbr></dfn> 是创建网页的标准标记语言。</p>
```

**4. 或者，添加 id 属性。 然后，无论何时使用一个术语，它都可以使用 \<a> 标签引用该定义：**

```html idoc:preview
<p><dfn id="html-def">HTML</dfn> 是创建网页的标准标记语言。</p>

<p>This is some text...</p>
<p>This is some text...</p>
<p>Learn <a href="#html-def">HTML</a> now.</p>
```
<!--rehype:style=min-height: 180px;-->

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| \<dfn>  | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<dfn>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<dfn>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<dfn>` 元素：

```css
dfn {
  font-style: italic;
}
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg