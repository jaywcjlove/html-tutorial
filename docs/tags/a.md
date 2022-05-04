HTML \<a> 标签
===

## 示例

指向 github.com 的超链接：

```html idoc:preview
<a target="_blank" href="https://github.com/jaywcjlove">HTML Tutorial</a>
```

## 定义和用法

`<a>` 标签定义了一个超链接，用于从一个页面链接到另一个页面。`<a>` 元素最重要的属性是 `href` 属性，它指示链接的目的地。

默认情况下，链接将在所有浏览器中显示如下：

- _未访问的链接带有下划线和蓝色_ <!--rehype:style=color: #0000ff; text-decoration: underline;-->
- _访问过的链接带有下划线和紫色_ <!--rehype:style=color: purple; text-decoration: underline;-->
- _活动链接带有下划线和红色_ <!--rehype:style=color: red; text-decoration: underline;-->

## 属性

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [download](./a_download.md) | filename | 指定当用户单击超链接时将下载目标 |
| [href](./a_href.md) | URL | 指定链接指向的页面的 URL |
| [hreflang](./a_hreflang.md) | language_code | 指定链接文档的语言 |
| [media](./a_media.md) | media_query | 指定链接文档针对什么媒体/设备进行优化 |
| [ping](./a_ping.md) | list_of_URLs | 指定一个以空格分隔的 URL 列表，当点击链接时，浏览器将发送带有正文 ping 的 post 请求（在后台）。 通常用于跟踪 |
| [referrepolicy](./a_referrepolicy.md) | no-referrer,<br />no-referrer-when-downgrade,<br />origin,<br />origin-when-cross-origin,<br />same-origin,<br />strict-origin-when-cross-origin,<br />unsafe-url | 指定与链接一起发送的推荐人信息 |
| [rel](./a_rel.md) | alternate,<br />author,<br />bookmark,<br />external,<br />help,<br />license,<br />next,<br />nofollow,<br />noreferrer,<br />noopener,<br />prev,<br />search,<br />tag | 指定当前文档和链接文档之间的关系 |
| [target](./a_target.md) | _blank,<br />_parent,<br />_self,<br />_top | 指定打开链接文档的位置 |
| [type](./a_type.md) | media_type | 指定链接文档的媒体类型 |

## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;a&gt;__ | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

所有浏览器都支持 `<a>` 标签。

## 全局属性

`<a>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<a>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 更多示例

### 将图像作为链接

本例演示如何使用图像作为链接。

```html idoc:preview
<a href="https://github.com/jaywcjlove/html-tutorial">
  <img alt="HTML Tutorial" src="https://avatars1.githubusercontent.com/u/1680273?s=460&v=4" width="100" height="100">
</a>
```

### 在新的浏览器窗口打开链接

本例演示如何在新窗口打开一个页面，这样的话访问者就无需离开你的站点了。

```html idoc:preview
<a target="_blank" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

### 链接到电子邮件地址

本例演示如何如何链接到一个邮件。（本例在安装邮件客户端程序后才能工作。）

```html idoc:preview
<a href="mailto:someone@example.com">Send email</a>
<a href="mailto:someone@microsoft.com?cc=someoneelse@microsoft.com&bcc=andsomeoneelse2@microsoft.com&subject=Summer%20Party&body=You%20are%20invited%20to%20a%20big%20summer%20party!">发送邮件！</a>
```

### 链接电话号码

```html idoc:preview
<a href="tel:+8602122278911">+86 021-22278911</a>
```

### 描点链接

链接到同一页面上的另一个部分，页面自定定位到对应位置：

```html idoc:preview
<a href="#更多示例">跳转到当前页面的 "id=更多示例" 的位置</a>
```

### 执行 JS 脚本

```html idoc:preview
<a href="javascript:alert('Hello World!');">执行 JavaScript</a>
```

## 全局属性

`<a>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<a>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<a>` 元素：

```css
a:link, a:visited {
  color: (internal value);
  text-decoration: underline;
  cursor: auto;
}

a:link:active, a:visited:active {
  color: (internal value);
}
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg