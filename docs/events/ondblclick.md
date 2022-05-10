HTML ondblclick 事件属性
===

鼠标双击元素触发

## 示例

双击按钮时执行 JavaScript：

```html idoc:preview:iframe
<button ondblclick="myFunction()">双击我</button>
<p id="demo"></p>
<p>双击按钮时触发一个函数。 该函数在 id="demo" 的 p 元素中输出一些文本。</p>
<script>
  function myFunction() {
    document.getElementById("demo").innerHTML = "Hello World";
  }
</script>
```

```html
<button ondblclick="myFunction()">双击我</button>
```

## 定义和使用

`ondblclick` 属性在鼠标双击元素时触发。

## 浏览器支持

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| `ondblclick` | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element ondblclick="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 `ondblclick` 上运行的脚本 |

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | 所有 HTML 元素，除了: [\<base>](../tags/base.md), [\<bdo>](../tags/bdo.md), [\<br>](../tags/br.md), [\<head>](../tags/head.md), [\<html>](../tags/html.md), [\<iframe>](../tags/iframe.md), [\<meta>](../tags/meta.md), [\<param>](../tags/param.md), [\<script>](../tags/script.md), [\<style>](../tags/style.md), 和 [\<title>](../tags/title.md) |

## 更多示例

双击 \<p> 元素将其文本颜色更改为红色：

```html idoc:preview:iframe
<p id="demo" ondblclick="myFunction()">双击我以更改我的文本颜色。</p>

<p>双击 p 元素时触发一个函数。 该函数将 p 元素的颜色设置为红色。</p>

<script>
function myFunction() {
  document.getElementById("demo").style.color = "red";
}
</script>
```

```html
<p id="demo" ondblclick="myFunction()">双击我以更改我的文本颜色。</p>
<script>
  function myFunction() {
    document.getElementById("demo").style.color = "red";
  }
</script>
```

双击一个按钮将一些文本从一个输入字段复制到另一个输入字段：

```html idoc:preview:iframe
Field1: <input type="text" id="field1" value="Hello World!"><br>
Field2: <input type="text" id="field2"><br><br>

<button ondblclick="myFunction()">复制文本</button>
<p>双击按钮时触发一个函数。 该函数将文本从 Field1 复制到 Field2。</p>

<script>
function myFunction() {
  document.getElementById("field2").value = document.getElementById("field1").value;
}
</script>
```

```html
<button ondblclick="myFunction()">复制文本</button>
<script>
  function myFunction() {
    document.getElementById("field2").value = document.getElementById("field1").value;
  }
</script>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

