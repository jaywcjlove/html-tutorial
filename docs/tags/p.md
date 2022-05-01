HTML \<p> 标签
===

## 示例

一个段落标记如下：

```html idoc:preview
<p>这是段落中的一些文本</p>
```

## 定义和用法

`<p>` 标签定义了一个段落。

浏览器会自动在每个 `<p>` 元素之前和之后添加一个空行。

**提示：** 使用 CSS [样式段落](../tutorial/css.md)。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<p>    | Yes | Yes | Yes | Yes | Yes |

## 全局属性

`<p>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<p>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例

对齐段落中的文本（使用 CSS）：

```html idoc:preview
<p style="text-align:right">这是段落中的一些文本。</p>
```

使用 CSS 设置段落样式：

```html idoc:preview:iframe
<html>
<head>
  <style>
    p {
      color: navy;
      text-indent: 30px;
      text-transform: uppercase;
    }
  </style>
</head>
<body>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
</body>
</html>
```

更多关于段落：

```html idoc:preview:iframe
<p>
本段
包含很多行
在源代码中，
但是浏览器
忽略它。
</p>
```
<!--rehype:style=height: 30px;-->

HTML中的诗歌问题：

```html idoc:preview:iframe
<p>
北国风光，千里冰封，万里雪飘。
望长城内外，惟余莽莽；大河上下，顿失滔滔。
山舞银蛇，原驰蜡象，欲与天公试比高。
须晴日，看红装素裹，分外妖娆。
江山如此多娇，引无数英雄竞折腰。
惜秦皇汉武，略输文采；唐宗宋祖，稍逊风骚。
一代天骄，成吉思汗，只识弯弓射大雕。
俱往矣，数风流人物，还看今朝。
<em>---毛泽东</em>
</p>
```
<!--rehype:style=height: 130px;-->

## 相关页面

HTML 教程: [HTML Paragraphs](../tutorial/paragraphs.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<p>` 元素：

```css
p {
  display: block;
  margin-top: 1em;
  margin-bottom: 1em;
  margin-left: 0;
  margin-right: 0;
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg