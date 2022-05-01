HTML \<ol> Tag
===

## 示例

两个不同的有序列表（第一个列表从 1 开始，第二个从 50 开始）：

```html idoc:preview:iframe
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

## 定义和用法

`<ol>` 标签定义了一个有序列表。 有序列表可以是数字的或字母的。

[\<li>](./li.md) 标记用于定义每个列表项。

**提示：** 对于无序列表，使用 [\<ul>](./ul.md) 标签。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<ol>   | Yes | Yes | Yes | Yes | Yes |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [reversed](./ol_reversed.md) | reversed  | 指定应颠倒列表顺序 (9,8,7...) |
| [start](./ol_start.md)       | *number*  | 指定有序列表的起始值 |
| [type](./ol_type.md)         | `1` `A` `a` `I` `i` | 指定要在列表中使用的标记类型 |

## 全局属性

`<ol>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<ol>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


## 更多示例

设置不同的列表类型（使用 CSS）：

```html idoc:preview:iframe
<ol style="list-style-type:upper-roman">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol style="list-style-type:lower-alpha">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
<!--rehype:style=height: 230px;-->

显示 CSS 可用的所有不同列表类型：

```html
<style>
ol.a {list-style-type: armenian;}
ol.b {list-style-type: cjk-ideographic;}
ol.c {list-style-type: decimal;}
ol.d {list-style-type: decimal-leading-zero;}
ol.e {list-style-type: georgian;}
ol.f {list-style-type: hebrew;}
ol.g {list-style-type: hiragana;}
ol.h {list-style-type: hiragana-iroha;}
ol.i {list-style-type: katakana;}
ol.j {list-style-type: katakana-iroha;}
ol.k {list-style-type: lower-alpha;}
ol.l {list-style-type: lower-greek;}
ol.m {list-style-type: lower-latin;}
ol.n {list-style-type: lower-roman;}
ol.o {list-style-type: upper-alpha;}
ol.p {list-style-type: upper-latin;}
ol.q {list-style-type: upper-roman;}
ol.r {list-style-type: none;}
ol.s {list-style-type: inherit;}
</style>
```

带有 CSS 的 ol 的所有不同列表类型

```html idoc:preview:iframe
<!DOCTYPE html>
<html>
<head>
  <style>
    ol.a { list-style-type: armenian; }
    ol.b { list-style-type: cjk-ideographic; }
    ol.c { list-style-type: decimal; }
    ol.d { list-style-type: decimal-leading-zero; }
    ol.e { list-style-type: georgian; }
    ol.f { list-style-type: hebrew; }
    ol.g { list-style-type: hiragana; }
    ol.h { list-style-type: hiragana-iroha; }
    ol.i { list-style-type: katakana; }
    ol.j { list-style-type: katakana-iroha; }
    ol.k { list-style-type: lower-alpha; }
    ol.l { list-style-type: lower-greek; }
    ol.m { list-style-type: lower-latin; }
    ol.n { list-style-type: lower-roman; }
    ol.o { list-style-type: upper-alpha; }
    ol.p { list-style-type: upper-latin; }
    ol.q { list-style-type: upper-roman; }
    ol.r { list-style-type: none; }
    ol.s { list-style-type: inherit; }
  </style>
</head>
<body>
  <ol class="a">
    <li>Armenian type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="b">
    <li>Cjk-ideographic type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="c">
    <li>Decimal type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="d">
    <li>Decimal-leading-zero type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="e">
    <li>Georgian type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="f">
    <li>Hebrew type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="g">
    <li>Hiragana type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="h">
    <li>Hiragana-iroha type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="i">
    <li>Katakana type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="j">
    <li>Katakana-iroha type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="k">
    <li>Lower-alpha type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="l">
    <li>Lower-greek type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="m">
    <li>Lower-latin type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="n">
    <li>Lower-roman type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="o">
    <li>Upper-alpha type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="p">
    <li>Upper-latin type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="q">
    <li>Upper-roman type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="r">
    <li>None type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
  <ol class="s">
    <li>inherit type</li>
    <li>Tea</li>
    <li>Coca Cola</li>
  </ol>
</body>
</html>
```
<!--rehype:style=height: 230px;-->

减少和扩大列表中的行高（使用 CSS）：

```html idoc:preview:iframe
<ol style="line-height:80%">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol style="line-height:180%">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
<!--rehype:style=height: 230px;-->

在有序列表中嵌套一个无序列表：


```html idoc:preview:iframe
<ol>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ol>
```
<!--rehype:style=height: 230px;-->

## 相关页面

HTML 教程: [HTML Lists](../tutorial/lists.md)

## 默认 CSS 设置

大多数浏览器将显示具有以下默认值的 `<ol>` 元素：

```css
ol {
  display: block;
  list-style-type: decimal;
  margin-top: 1em;
  margin-bottom: 1em;
  margin-left: 0;
  margin-right: 0;
  padding-left: 40px;
}
```
<!--rehype:style=height: 230px;-->

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg