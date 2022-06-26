HTML onchange 属性
===

## 定义和用法

`onchange` 属性会在元素的值发生更改时触发。

**提示：** 此事件类似于 `oninput` 事件。 不同之处在于，`oninput` 事件会在元素的值发生更改后立即发生，而 `onchange` 会在元素失去焦点时发生。 另一个区别是 `onchange` 事件也适用于 `<select>` 元素。

## 适用于

`onchange` 属性是 [事件属性](../reference/attributes.md) 的一部分，可用于任何 HTML 元素。

| 元素 | 事件 |
| --- | --- |
| 所有 HTML 元素 | [onchange](../events/onchange.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 示例

### Select 示例

当用户更改 \<select> 元素的选定选项时执行 JavaScript：


```html
<select onchange="myFunction()">
```

```html idoc:preview:iframe
<select id="mySelect" onchange="myFunction()">
  <option value="Audi">Audi
  <option value="BMW">BMW
  <option value="Mercedes">Mercedes
  <option value="Volvo">Volvo
</select>
<p>
  当您选择一辆新车时，会触发一个函数，该函数会输出所选汽车的值。
</p>
<p id="demo"></p>
<script>
function myFunction() {
  var x = document.getElementById("mySelect").value;
  document.getElementById("demo").innerHTML = "You selected: " + x;
}
</script>
```

### Input 示例

当用户更改输入字段的内容时执行 JavaScript：

```html
<input type="text" name="txt" value="Hello" onchange="myFunction(this.value)">
```

```html idoc:preview:iframe
<p>
  修改输入字段中的文本，然后在字段外单击以触发 onchange 事件。
</p>
输入一些文字：<input type="text" name="txt" value="Hello" onchange="myFunction(this.value)">
<p id="demo"></p>
<script>
function myFunction(val) {
  console.log('~~~')
  document.getElementById("demo").innerHTML = "输入值已更改。 新值是：" + val;
}
</script>
```

## 浏览器支持

| 元素 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onchange        | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

