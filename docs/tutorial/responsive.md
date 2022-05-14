HTML 响应式网页设计
===

响应式网页设计是关于创建在所有设备上看起来都不错的网页！

响应式网页设计将自动调整不同的屏幕尺寸和视口。

## 什么是响应式网页设计？

响应式网页设计是关于使用 HTML 和 CSS 自动调整网站大小、隐藏、缩小或放大网站，使其在所有设备（台式机、平板电脑和手机）上看起来都不错：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * { box-sizing: border-box; }
    .menu {
      float: left;
      width: 20%;
    }
    .menuitem {
      padding: 8px;
      margin-top: 7px;
      border-bottom: 1px solid #f1f1f1;
    }
    .main {
      float: left;
      width: 60%;
      padding: 0 20px;
      overflow: hidden;
    }
    .right {
      background-color: lightblue;
      float: left;
      width: 20%;
      padding: 10px 15px;
      margin-top: 7px;
    }

    @media only screen and (max-width:800px) {
      /* For tablets: */
      .main {
        width: 80%;
        padding: 0;
      }
      .right {
        width: 100%;
      }
    }
    @media only screen and (max-width:500px) {
      /* For mobile phones: */
      .menu, .main, .right {
        width: 100%;
      }
    }
  </style>
</head>
<body style="font-family:Verdana;">
  <div style="background-color:#f1f1f1;padding:15px;">
    <h1>上海市</h1>
    <h3>调整浏览器窗口大小</h3>
  </div>

  <div style="overflow:auto">
    <div class="menu">
      <div class="menuitem">青浦区</div>
      <div class="menuitem">黄浦区</div>
      <div class="menuitem">浦东新区</div>
      <div class="menuitem">宝山区</div>
    </div>

    <div class="main">
      <h2>青浦区</h2>
      <p>青浦区，中国上海市市辖区，位于上海市西部，太湖下游，黄浦江上游。东与闵行区毗邻，南与松江区、金山区及浙江省嘉兴市嘉善县接壤，西与江苏省苏州市吴江区、苏州市昆山市相连，北与嘉定区相接。青浦区下辖3街道、8镇，总面积668.54平方公里</p>
    </div>
  </div>

  <div style="background-color:#f1f1f1;text-align:center;padding:10px;margin-top:7px;font-size:12px;">该网页是流畅网页设计演示的一部分。 调整浏览器窗口大小以查看内容对调整大小的响应。</div>
</body>
</html>
```
<!--rehype:style=height: 430px;-->

## 设置 viewport

要创建响应式网站，请将以下 [`<meta>`](../tags/meta.md) 标签添加到您的所有网页：

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <h2>Setting the Viewport</h2>
  <p>这个例子并没有真正做任何事情，除了向您展示如何添加视口元元素.</p>
</body>
</html>
```

这将设置页面的视口，这将为浏览器提供有关如何控制页面尺寸和缩放的说明。

这是一个没有 viewport 元标签的网页示例，以及具有 viewport 元标签的同一网页：

没有 viewport 元标签 | 使用 viewport 元标签
---- | ----
![](../assets/responsive_viewport1.png) | ![](../assets/responsive_viewport2.png)

## 响应式图像

响应式图像是可以很好地缩放以适应任何浏览器大小的图像。

![](../assets/example.png)

注意：上面图片是原始尺寸，下面有三种方法实现响应式图像。

### 使用 width 属性

如果 CSS 的 `width` 属性设置为 100%，图像将响应并放大和缩小：

```html idoc:preview
<img src="../assets/example.png" style="width:100%;">
```
<!--rehype:style=height: 230px;-->

请注意，在上面的示例中，图像可以放大到大于其原始大小。 在许多情况下，更好的解决方案是使用 `max-width` 属性。

### 使用 max-width 属性

如果 `max-width` 属性设置为 100%，则图像将在必要时缩小，但永远不会放大到大于其原始尺寸：

```html idoc:preview
<img src="../assets/example.png" style="max-width:100%;height:auto;">
```
<!--rehype:style=height: 230px;-->

### 根据浏览器宽度显示不同的图像

HTML [`<picture>`](../tags/picture.md) 元素允许您为不同的浏览器窗口大小定义不同的图像。

调整浏览器窗口大小以查看下图如何根据宽度变化：

```html idoc:preview
<picture>
  <source srcset="../assets/example.png" media="(max-width: 600px)">
  <source srcset="../assets/sublime_text.png" media="(max-width: 1500px)">
  <source srcset="../assets/chrome.svg">
  <img src="../assets/example.png" alt="Flowers">
</picture>
```

## 响应式文本大小

可以使用 `vw` 单位设置文本大小，即 `viewport width`。

这样，文本大小将跟随浏览器窗口的大小：

```html idoc:preview
<h1 style="font-size:8vw;">Hello World</h1>
<p style="font-size:2vw;">调整浏览器窗口的大小以查看文本大小的缩放方式。</p>
```
<!--rehype:style=height: 360px;-->

标题字体调整

```html idoc:preview
<h1 style="font-size:10vw;">Hello World</h1>
```
<!--rehype:style=height: 360px;-->

视口是浏览器窗口的大小。 1vw = 视口宽度的 1%。 如果视口为 50 厘米宽，则 1vw 为 0.5 厘米。

## 媒体查询

除了调整文本和图像的大小之外，在响应式网页中使用媒体查询也很常见。

使用媒体查询，您可以为不同的浏览器尺寸定义完全不同的样式。

示例：调整浏览器窗口大小，可以看到下面三个 div 元素会在大屏上水平显示，在小屏上垂直堆叠：

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
  * { box-sizing: border-box; }
  .left {
    background-color: #2196F3;
    padding: 20px;
    float: left;
    width: 20%; /* 默认情况下，宽度为 20% */
  }
  .main {
    background-color: #f1f1f1;
    padding: 20px;
    float: left;
    width: 60%; /* 默认情况下，宽度为 60% */
  }
  .right {
    background-color: #04AA6D;
    padding: 20px;
    float: left;
    width: 20%; /* 默认情况下，宽度为 20% */
  }
  /* 使用媒体查询在 800 像素处添加断点： */
  @media screen and (max-width: 600px) {
    .left, .main, .right {
      width: 100%; /* 当视口为 800px 或更小时，宽度为 100% */
    }
  }
</style>
</head>
<body>
  <p>调整浏览器窗口的大小。</p>
  <p>确保在调整此帧大小时到达 800px 处的断点。</p>
  <div class="left">
    <p>Left Menu</p>
  </div>
  <div class="main">
    <p>Main Content</p>
  </div>
  <div class="right">
    <p>Right Content</p>
  </div>
</body>
</html>
```
<!--rehype:style=height: 260px;-->

## 响应式网页 - 完整示例

响应式网页在大型桌面屏幕和小型手机上应该看起来不错。

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
  * { box-sizing: border-box; }
  .menu {
    float: left;
    width: 20%;
    text-align: center;
  }
  .menu a {
    background-color: #e5e5e5;
    padding: 8px;
    margin-top: 7px;
    display: block;
    width: 100%;
    color: black;
  }
  .main {
    float: left;
    width: 60%;
    padding: 0 20px;
  }
  .right {
    background-color: #e5e5e5;
    float: left;
    width: 20%;
    padding: 15px;
    margin-top: 7px;
    text-align: center;
  }

  @media only screen and (max-width: 520px) {
    /* For mobile phones: */
    .menu, .main, .right {
      width: 100%;
    }
  }
  </style>
</head>
<body style="font-family:Verdana;color:#aaaaaa;">
  <div style="background-color:#e5e5e5;padding:15px;text-align:center;">
    <h1>Hello World</h1>
  </div>

  <div style="overflow:auto">
    <div class="menu">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
      <a href="#">Link 4</a>
    </div>

    <div class="main">
      <h2>HTML Tutorial</h2>
      <p>HTML（超文本标记语言——HyperText Markup Language）是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）。</p>
    </div>

    <div class="right">
      <h2>关于</h2>
      <p>HTML Tutorial</p>
    </div>
  </div>
  <div style="background-color:#e5e5e5;text-align:center;padding:10px;margin-top:7px;">© HTML Tutorial</div>
</body>
</html>
```
<!--rehype:style=height: 360px;-->

## 响应式网页设计 - 框架

所有流行的 CSS 框架都提供响应式设计。

它们是免费的，并且易于使用。

### Bootstrap

另一个流行的 CSS 框架是 [Bootstrap](https://getbootstrap.com/)。 Bootstrap 使用 HTML、CSS 和 jQuery 来制作响应式网页。

```html idoc:preview:iframe
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css">
  <script src="https://cdn.jsdelivr.net/npm/jquery@3.6.0/dist/jquery.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.min.js"></script>
</head>
<body>
  <div class="container">
    <div class="jumbotron">
      <h1>我的第一个 Bootstrap 页面</h1>
    </div>
    <div class="row">
      <div class="col-sm">
        左边内容...
      </div>
      <div class="col-sm">
        中间内容...
      </div>
      <div class="col-sm">
        右边内容...
      </div>
    </div>
  </div>
</body>
</html>
```
<!--rehype:style=height: 200px;-->