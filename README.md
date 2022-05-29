HTML Tutorial
===

HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）。

“超文本”（hypertext）是指连接单个网站内或多个网站间的网页的链接。链接是网络的一个基本方面。只要将内容上传到互联网，并将其与他人创建的页面相链接，你就成为了万维网的积极参与者。

HTML 使用“标签”（markup）来注明文本、图片和其他内容，以便于在 Web 浏览器中显示。

HTML 元素通过“标签”（tag）将文本从文档中引出，标签由在 `<` 和 `>` 中包裹的元素名组成，HTML 标签里的元素名不区分大小写。也就是说，它们可以用大写，小写或混合形式书写。例如，`<title>` 标签可以写成 `<Title>`，`<TITLE>` 或以任何其他方式。

```html
<title>标题</title>
<TITLE>标题</TITLE>
```

```bash
                    ╭┈┈┈┈┈┈┈┈┈┈┈╮
                    ┆  Element  ┆
                    ╰┈┈┈┈┈┬┈┈┈┈┈╯
                          ▼ 
     ╭┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╮
  开始标签              文本内容               结束标签
     ▼               ╰┈┈┈┈┬┈┈┈┈╯               ▼
╭┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈╮
┆ <div class="ab">   this my content        </div>  ┆
╰┈┈┈┈┈┈╱┈┈┈┈┈┈┈┈╲┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╲┈┈┈┈┈╯
   属性名称      属性值                    注意结束“/”符号
    name        value
     ╰┈┈┈┈┈┈┬┈┈┈┈┈╯
     Attribute(属性)
```

教程、参考资料和示例会不断审查以避免错误，但不能保证所有内容的完全正确性，所有资源来源网络。

## HTML 简史

在 1980 年代后期，作为 CERN 承包商的物理学家 Tim Berners-Lee 为 CERN 研究人员提出了一个系统。 1989 年，他写了一份备忘录，提出了一个基于互联网的超文本系统。

Tim Berners-Lee 被称为 HTML 之父。 HTML 的第一个可用描述是 Tim 在 1991 年末提出的名为“HTML 标签”的文档。HTML 的最新版本是 HTML5，我们将在本教程的后面部分学习。


| Year | Version |
| ---- | ---- |
| 1989 | Tim Berners-Lee 发明了 www |
| 1991 | Tim Berners-Lee 发明了 HTML |
| 1993 | Dave Raggett 起草了 HTML+ |
| 1995 | HTML 工作组定义的 HTML 2.0 |
| 1997 | W3C Recommendation: HTML 3.2 |
| 1999 | W3C Recommendation: HTML 4.01 |
| 2000 | W3C Recommendation: XHTML 1.0 |
| 2008 | WHATWG HTML5 首次公开草案 |
| 2012 | [WHATWG HTML5 Living Standard](http://whatwg.org/html/) |
| 2014 | [W3C Recommendation: HTML5](http://www.w3.org/TR/html5/) |
| 2016 | W3C Candidate Recommendation: HTML 5.1 |
| 2017 | [W3C Recommendation: HTML5.1 2nd Edition](http://www.w3.org/TR/html51/) |
| 2017 | [W3C Recommendation: HTML5.2](http://www.w3.org/TR/html52/) |


## HTML 要点

- HTML 代表超文本标记语言。
- HTML 用于创建网页和 Web 应用程序。
- HTML 是网络上广泛使用的语言。
- 我们只能通过 HTML 创建静态网站。
- 从技术上讲，HTML 是一种标记语言，而不是一种编程语言。

## HTML 版本

自 HTML 发明以来，市场上有很多 HTML 版本，下面对 HTML 版本进行简单介绍：

**① HTML 1.0：** HTML 的第一个版本是 1.0，它是 HTML 语言的准系统版本，于 1991 年发布。

**② HTML 2.0：** 这是 1995 年发布的下一个版本，是网站设计的标准语言版本。 HTML 2.0 能够支持额外的功能，例如基于表单的文件上传、文本框等表单元素、选项按钮等。

**③ HTML 3.2：** HTML 3.2 版本由 W3C 于 1997 年初发布。此版本能够创建表格并为表单元素的额外选项提供支持。 它还可以支持具有复杂数学方程的网页。 直到 1997 年 1 月，它才成为任何浏览器的官方标准。如今，大多数浏览器实际上都支持它。

**④ HTML 4.01：** HTML 4.01 版本于 1999 年 12 月发布，是一个非常稳定的 HTML 语言版本。 这个版本是当前的官方标准，它增加了对样式表 (CSS) 的支持和各种多媒体元素的脚本能力。

**⑤ HTML 5：** HTML 5 是超文本标记语言的最新版本。 该版本的初稿于 2008 年 1 月公布。有两个主要组织，一个是 [W3C](https://www.w3.org/)（万维网联盟），另一个是 [WHATWG](https://whatwg.org/)（Web 超文本应用技术工作组），它们参与了 HTML 5 版本的开发 ，并且仍在开发中。

<!--idoc:ignore:start-->

## 目录

- [HTML 索引 (字母排序)](./docs/tags/README.md)
- [HTML 索引 (分类)](./docs/reference/byfunc.md)
- [HTML 浏览器支持](./docs/reference/browsersupport.md)
- [HTML 属性参考](./docs/reference/attributes.md)
- [HTML 全局属性](./docs/reference/standardattributes.md)
- [HTML 事件](./docs/reference/eventattributes.md)
- [HTML 颜色名](./docs/reference/colornames.md)
- [HTML Canvas](./docs/reference/canvas.md)
- [HTML 音频/视频](./docs/reference/av_dom.md)
- [HTML 字符集(UTF-8)](./docs/reference/charactersets.md)
- [HTML 字符集实体(全)](./docs/reference/charactersets_entities.md)
- [HTML Doctypes](./docs/reference/dtd.md)
- [HTML URL 编码](./docs/reference/urlencode.md)
- [HTML 语言代码](./docs/reference/language_codes.md)
- [HTML 国家/地区代码](./docs/reference/country_codes.md)
- [HTTP 状态消息](./docs/reference/httpmessages.md)
- [键盘快捷键](./docs/reference/keyboardshortcuts.md)

<!--idoc:ignore:end-->

## Docker

```bash
docker pull wcjiang/html-tutorial
```

```bash
docker run --name html-tutorial --rm -d -p 9666:80 wcjiang/html-tutorial:latest
# Or
docker run --name html-tutorial -itd -p 9666:80 wcjiang/html-tutorial:latest
```

Visit the following URL in your browser

```bash
http://localhost:9666/
```

## Contributors

一如既往，感谢我们出色的贡献者！一天搬运一个慢慢攒吧，欢迎大家参与进来 :)。

<a href="https://github.com/jaywcjlove/html-tutorial/graphs/contributors">
  <img src="https://jaywcjlove.github.io/html-tutorial/CONTRIBUTORS.svg" />
</a>

Made with [action-contributors](https://github.com/jaywcjlove/github-action-contributors).

## License

Licensed under the MIT License.
