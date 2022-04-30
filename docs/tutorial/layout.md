HTML 布局元素和技术
===

网站通常在多个栏目中显示内容（如杂志或报纸）。

## 示例

```html idoc:preview:iframe
<style>
  * { box-sizing: border-box; }
  body { font-family: Arial, Helvetica, sans-serif; }
  header {
    background-color: #666;
    text-align: center;
    font-size: 35px;
    padding: 1px 30px;
    color: white;
  }
  nav {
    float: left;
    width: 30%;
    height: 280px;
    background: #ccc;
    padding: 20px;
  }
  nav ul {
    list-style-type: none;
    padding: 0;
  }
  article {
    float: left;
    padding: 20px;
    width: 70%;
    background-color: #f1f1f1;
    height: 280px;
  }
  section::after {
    content: "";
    display: table;
    clear: both;
  }
  footer {
    background-color: #777;
    padding: 10px;
    text-align: center;
    color: white;
  }
</style>
<div>
  <header class="header">
    <h2>Cities</h2>
  </header>
  <section class="section">
    <nav class="nav">
      <ul>
        <li><a href="javascript:void(0)">北京</a></li>
        <li><a href="javascript:void(0)">上海</a></li>
        <li><a href="javascript:void(0)">武汉</a></li>
      </ul>
    </nav>
    <article class="article">
      <h1>上海</h1>
      <p>上海，简称“沪”或“申”，是中华人民共和国省级行政区、直辖市、国家中心城市、超大城市、上海大都市圈核心城市，国务院批复确定的中国国际经济、金融、贸易、航运、科技创新中心 [1]  。截至2019年，全市下辖16个区，总面积6340.5平方千米，建成区面积1237.85平方千米。</p>
      <p>2021年末，全市常住人口为2489.43万人。 [192]  2021年，上海市地区生产总值43214.85亿元，GDP同比增长8.1%。</p>
    </article>
  </section>
  <footer class="footer"> 
    <p>Footer</p>
  </footer>
</div>
```
<!--rehype:style=height: 520px;-->

## HTML 布局元素

HTML 有几个语义元素来定义网页的不同部分：

```bash
╭┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╮
┆         <header>        ┆
├┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┤
┆           <nav>         ┆
┆┈┈┈┈┈┈┈┈┈┈┈┈┈┬┈┈┈┈┈┈┈┈┈┈┈┤
┆  <section>  ┆           ┆
┆┈┈┈┈┈┈┈┈┈┈┈┈┈┤  <aside>  ┆
┆  <article>  ┆           ┆
┆┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┤
┆         <footer>        ┆
╰┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╯
```
<!--rehype:style=float: left;margin-right: 16px;-->

`<header>` - 定义文档或部分的**标题**\
`<nav>` - 定义一组**导航**链接\
`<section>` - 定义文档中的一个部分\
`<article>` - 定义一个独立的、自包含的内容\
`<aside>` - 定义除内容之外的内容（如侧边栏）\
`<footer>` - 定义文档或部分的**页脚**\
`<details>` - 定义用户可以按需打开和关闭的其他**详细信息**\
`<summary>` - 定义 `<details>` 元素的**标题**

## HTML 布局技术
<!--rehype:style=clear: both;-->

有四种不同的技术可以创建多列布局。 每种技术都有其优点和缺点：

- CSS 框架
- CSS 浮动属性
- CSS 弹性盒
- CSS 网格

## CSS 框架

如果您想快速创建布局，可以使用 CSS 框架，例如 [Bootstrap](https://getbootstrap.com/)。

## CSS浮动布局

使用 CSS `float` 属性来做整个网页布局是很常见的。 Float 很容易学习——你只需要记住 `float` 和 `clear` 属性是如何工作的。

**缺点：** 浮动元素与文档流相关，可能会损害灵活性。

```html idoc:preview:iframe
<!DOCTYPE html>
<html lang="en">
<head>
  <style>
    * { box-sizing: border-box; }
    body { font-family: Arial, Helvetica, sans-serif; }
    header {
      background-color: #666;
      text-align: center;
      font-size: 35px;
      padding: 1px 30px;
      color: white;
    }
    nav {
      float: left;
      width: 30%;
      height: 280px;
      background: #ccc;
      padding: 20px;
    }
    nav ul {
      list-style-type: none;
      padding: 0;
    }
    article {
      float: left;
      padding: 20px;
      width: 70%;
      background-color: #f1f1f1;
      height: 280px;
    }
    section::after {
      content: "";
      display: table;
      clear: both;
    }
    footer {
      background-color: #777;
      padding: 10px;
      text-align: center;
      color: white;
    }
  </style>
</head>
<body>
  <header>
    <h2>Cities</h2>
  </header>
  <section>
    <nav>
      <ul>
        <li><a href="javascript:void(0)">北京</a></li>
        <li><a href="javascript:void(0)">上海</a></li>
        <li><a href="javascript:void(0)">武汉</a></li>
      </ul>
    </nav>
    <article>
      <h1>上海</h1>
      <p>上海，简称“沪”或“申”，是中华人民共和国省级行政区、直辖市、国家中心城市、超大城市、上海大都市圈核心城市，国务院批复确定的中国国际经济、金融、贸易、航运、科技创新中心。</p>
      <p>截至2019年，全市下辖16个区，总面积6340.5平方千米，建成区面积1237.85平方千米。</p>
    </article>
  </section>
  <footer>
    <p>Footer</p>
  </footer>
</body>
</html>
```
<!--rehype:style=height: 520px;-->

## CSS 弹性盒布局

使用 flexbox 可确保当页面布局必须适应不同的屏幕尺寸和不同的显示设备时元素的行为是可预测的。在下面示例中，我们创建了一个页眉、两个列/框和一个页脚。

```html idoc:preview:iframe
<!DOCTYPE html>
<html lang="en">
<head>
  <style>
    * { box-sizing: border-box; }
    body { font-family: Arial, Helvetica, sans-serif; }
    header {
      background-color: #666;
      padding: 30px;
      text-align: center;
      font-size: 35px;
      color: white;
    }
    section {
      display: -webkit-flex;
      display: flex;
    }
    nav {
      flex: 1;
      background: #ccc;
      padding: 20px;
    }
    nav ul {
      list-style-type: none;
      padding: 0;
    }
    article {
      flex: 3;
      background-color: #f1f1f1;
      padding: 10px;
    }
    footer {
      background-color: #777;
      padding: 10px;
      text-align: center;
      color: white;
    }
  </style>
</head>
<body>
  <header>
    <h2>Cities</h2>
  </header>
  <section>
    <nav>
      <ul>
        <li><a href="javascript:void(0)">北京</a></li>
        <li><a href="javascript:void(0)">上海</a></li>
        <li><a href="javascript:void(0)">武汉</a></li>
      </ul>
    </nav>
    <article>
      <h1>上海</h1>
      <p>上海，简称“沪”或“申”，是中华人民共和国省级行政区、直辖市、国家中心城市、超大城市、上海大都市圈核心城市，国务院批复确定的中国国际经济、金融、贸易、航运、科技创新中心。</p>
      <p>截至2019年，全市下辖16个区，总面积6340.5平方千米，建成区面积1237.85平方千米。</p>
    </article>
  </section>
  <footer>
    <p>Footer</p>
  </footer>
</body>
</html>
```
<!--rehype:style=height: 520px;-->

## CSS 网格布局

CSS 网格布局模块提供了一个基于网格的布局系统，具有行和列，使设计网页更容易，而无需使用浮动和定位。

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
  <head>
    <style>
      .item1 { grid-area: header; }
      .item2 { grid-area: menu; }
      .item3 { grid-area: main; }
      .item4 { grid-area: right; }
      .item5 { grid-area: footer; }
      .grid-container {
        display: grid;
        grid-template-areas:
          'header header header header header header'
          'menu main main main right right'
          'menu footer footer footer footer footer';
        gap: 10px;
        background-color: #2196F3;
        padding: 10px;
      }
      .grid-container > div {
        background-color: rgba(255, 255, 255, 0.8);
        text-align: center;
        padding: 20px 0;
        font-size: 30px;
      }
    </style>
  </head>
  <body>
    <div class="grid-container">
      <div class="item1">Header</div>
      <div class="item2">Menu</div>
      <div class="item3">Main</div>  
      <div class="item4">Right</div>
      <div class="item5">Footer</div>
    </div>
  </body>
</html>
```
<!--rehype:style=height: 330px;-->