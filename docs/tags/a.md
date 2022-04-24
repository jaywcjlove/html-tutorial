HTML `<a>` 标签
===

## 示例

指向 github.com 的超链接：

```html
<a href="https://github.com/jaywcjlove/html-tutorial">HTML Tutorial</a>
```

## 定义和用法

`<a>` 标签定义了一个超链接，用于从一个页面链接到另一个页面。`<a>` 元素最重要的属性是 `href` 属性，它指示链接的目的地。

默认情况下，链接将在所有浏览器中显示如下：

- _未访问的链接带有下划线和蓝色_ <!--rehype:style=color: #0000ff; text-decoration: underline;-->
- _访问过的链接带有下划线和紫色_ <!--rehype:style=color: purple; text-decoration: underline;-->
- _活动链接带有下划线和红色_ <!--rehype:style=color: red; text-decoration: underline;-->


## 浏览器支持

| &nbsp; | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| __&lt;a&gt;__ | Yes | Yes | Yes | Yes | Yes |

所有浏览器都支持 `<a>` 标签。

## 更多示例

### 将图像作为链接

本例演示如何使用图像作为链接。

```html
<a href="https://github.com/jaywcjlove/html-tutorial">
  <img alt="HTML Tutorial" src="https://avatars1.githubusercontent.com/u/1680273?s=460&v=4" width="100" height="100">
</a>
```

### 在新的浏览器窗口打开链接

本例演示如何在新窗口打开一个页面，这样的话访问者就无需离开你的站点了。

```html
<a target="_blank" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

### 链接到电子邮件地址

本例演示如何如何链接到一个邮件。（本例在安装邮件客户端程序后才能工作。）

```html
<a href="mailto:someone@example.com">Send email</a>
<a href="mailto:someone@microsoft.com?cc=someoneelse@microsoft.com&bcc=andsomeoneelse2@microsoft.com&subject=Summer%20Party&body=You%20are%20invited%20to%20a%20big%20summer%20party!">发送邮件！</a>
```

### 链接电话号码

```html
<a href="tel:+8602122278911">+86 021-22278911</a>
```

### 描点链接

链接到同一页面上的另一个部分，页面自定定位到对应位置：

```html
<a href="#section2">跳转到当前页面的 id=section2 的位置</a>
```

### 执行 JS 脚本

```html
<a href="javascript:alert('Hello World!');">执行 JavaScript</a>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg