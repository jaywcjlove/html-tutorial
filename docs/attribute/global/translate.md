HTML `translate` 属性
===

指定有关元素的额外信息。

## 实例

指定不应翻译某些元素：

```html idoc:preview
<p translate="no">不要翻译这个！</p>
<p>这可以翻译成任何语言。</p>
```

## 定义和使用

translate 属性指定是否应该翻译元素的内容。

测试：点击谷歌翻译图片（在页面顶部的搜索按钮旁边）切换到另一种语言，看看下面的“冰淇淋”这个词会发生什么：
<!--rehype:style=color:#ff5722;-->

这里我们使用 translate="no": <span translate="no">冰淇淋</span>。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;title&gt;__ | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 | ❌ 不支持 |

## 语法

```html
<element translate="yes|no">
```

## 属性值

值 Value | 描述 Description
---- | ----
yes | 指定应该翻译元素的内容
no | 指定元素的内容不能被翻译

[1]: ../../assets/chrome.svg
[2]: ../../assets/edge.svg
[3]: ../../assets/firefox.svg
[4]: ../../assets/safari.svg
[5]: ../../assets/opera.svg