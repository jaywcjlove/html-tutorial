HTML `<a>` 标签的 rel 属性
===

## 示例

带有 rel 属性的链接：

```html idoc:preview
<a rel="nofollow" href="https://github.com/jaywcjlove/html-tutorial">HTML Tutorial</a>
```

## 定义和用法

`rel` 属性指定当前文档和链接文档之间的关系。

仅在存在 `href` 属性时使用。

**提示：** 搜索引擎可以使用此属性来获取有关链接的更多信息！

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| rel       | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<a rel="value">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| alternate  | 提供指向文档替代表示的链接（即打印页面、翻译或镜像） |
| author     | 提供指向文档作者的链接 |
| bookmark   | 用于书签的永久 URL |
| external   | 表示引用的文档与当前文档不属于同一站点 |
| help       | 提供指向帮助文档的链接 |
| license    | 提供指向文档许可信息的链接 |
| next       | 提供指向系列中下一个文档的链接 |
| nofollow   | 指向未经认可的文档的链接，例如付费链接。 （Google 使用“nofollow”来指定 Google 搜索蜘蛛不应跟随该链接） |
| noopener   | 要求通过超链接创建的任何浏览上下文都不能有开启者浏览上下文 |
| noreferrer | 使引用者未知。用户点击超链接时不包含referer header |
| prev       | 选择中的上一个文档 |
| search     | 指向文档搜索工具的链接 |
| tag        | 当前文档的标签（关键字） |



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg