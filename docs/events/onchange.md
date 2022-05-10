HTML onchange 事件属性
===

当元素的值改变时触发

## 示例

当用户更改 \<select> 元素的选定选项时执行 JavaScript：

```html idoc:preview:iframe
<select id="mySelect" onchange="myFunction()">
  <option value="Audi">奥迪
  <option value="BMW">宝马
  <option value="Mercedes">梅赛德斯
  <option value="Volvo">沃尔沃
</select>
<p>当您选择一辆新车时，会触发一个函数，该函数会输出所选汽车的值。</p>
<p id="demo"></p>
<script>
function myFunction() {
  var x = document.getElementById("mySelect").value;
  document.getElementById("demo").innerHTML = "You selected: " + x;
}
</script>
```


## 定义和使用

`onchange` 属性会在元素的值发生更改时触发。

**提示：** 此事件类似于 [oninput](./oninput.md) 事件。 不同之处在于，oninput 事件在元素的值发生更改后立即发生，而 `onchange` 在元素失去焦点时发生。 另一个区别是 `onchange` 事件也适用于 \<select> 元素。

## 浏览器支持

表中的数字指定了第一个完全支持事件属性的浏览器版本。

| 事件属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| --- | --- | --- | --- | --- | --- |
| onchange        | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<element onchange="script">
```

## 属性值

| 值 Value | 描述 Description |
| --- | --- |
| *script* | 要在 onchange 上运行的脚本 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 技术细节

|   |   |
| ---- | ---- |
| 支持的 HTML 标签: | [\<input type="checkbox">](../tags/input_type_checkbox.md), [\<input type="file">](../tags/input_type_file.md), [\<input type="password">](../tags/input_type_password.md), [\<input type="radio">](../tags/input_type_radio.md), [\<input type="range">](../tags/input_type_range.md), [\<input type="search">](../tags/input_type_search.md), [\<input type="text">](../tags/input_type_text.md), [\<select>](../tags/select.md), [\<textarea>](../tags/textarea.md) |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

当用户更改输入字段的内容时执行 JavaScript：

```html idoc:preview:iframe
修改输入字段中的文本，然后在 Input 输入框外单击以触发 onchange 事件。<br>
输入一些文字：<input type="text" name="txt" value="Hello" onchange="myFunction(this.value)">
<p id="demo"></p>
<script>
function myFunction(val) {
  document.getElementById("demo").innerHTML = "您输入了: " + val;
}
</script>
```



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

