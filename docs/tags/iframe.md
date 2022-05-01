HTML \<iframe> 标签
===

## 示例

内联框架标记如下：

```html idoc:preview
<iframe src="./html.html" title="HTML Tutorial" height="100%" width="100%"></iframe>
```
<!--rehype:style=min-height: 260px;-->

## 定义和用法

`<iframe>` 标签指定内联框架。

内联框架用于在当前 HTML 文档中嵌入另一个文档。

**提示：** 使用 CSS 设置 `<iframe>` 的样式（参见下面的示例）。

**提示：** 最好始终包含 `<iframe>` 的标题属性。 屏幕阅读器使用它来读取 `<iframe>` 的内容。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<iframe> | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| allow |   | 为 \<iframe> 指定功能策略 |
| allowfullscreen | true <br /> false | 如果 \<iframe> 可以通过调用 requestFullscreen() 方法激活全屏模式，则设置为 true |
| allowpaymentrequest | true <br /> false | 如果应允许跨域 \<iframe> 调用支付请求 API，则设置为 true |
| [height](./iframe_height.md) | *pixels* | 指定 \<iframe> 的高度。 默认高度为 150 像素 |
| loading | eager <br /> lazy | 指定浏览器是应该立即加载 iframe 还是推迟加载 iframe 直到满足某些条件 |
| [name](./iframe_name.md) | *text* | 指定 \<iframe> 的名称 |
| [referrerpolicy](./iframe_referrerpolicy.md) | no-referrer<br />no-referrer-when-downgrade<br />origin<br />origin-when-cross-origin<br />same-origin<br />strict-origin-when-cross-origin<br />unsafe-url | 指定在获取 iframe 时要发送的引荐来源网址信息 |
| [sandbox](./iframe_sandbox.md) | allow-forms<br />allow-pointer-lock<br />allow-popups<br />allow-same-origin<br />allow-scripts<br />allow-top-navigation | 为 \<iframe> 中的内容启用一组额外的限制 |
| [src](./iframe_src.md) | *URL* | 指定要嵌入到 \<iframe> 中的文档的地址 |
| [srcdoc](./iframe_srcdoc.md) | *HTML\_code* | 指定要在 \<iframe> 中显示的页面的 HTML 内容 |
| [width](./iframe_width.md) | *pixels* | 指定 \<iframe> 的宽度。 默认宽度为 300 像素 |

## 全局属性

`<iframe>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<iframe>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

添加和删除 iframe 边框（使用 CSS）：

```html idoc:preview
<iframe src="./header.html" width="100%" height="300" style="border:1px solid black;"></iframe>

<iframe src="./header.html" width="100%" height="300" style="border:none;"></iframe>
```
<!--rehype:style=min-height: 260px;-->

## 相关页面

HTML 教程: [HTML Iframes](../tutorial/iframe.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<iframe>` 元素：

```css
iframe:focus {
  outline: none;
}
iframe[seamless] {
  display: block;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg