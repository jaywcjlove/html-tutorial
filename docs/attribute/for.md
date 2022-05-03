HTML for 属性
===

## 定义和用法

当与 [`<label>`](../tags/label.md) 元素一起使用时，`for` 属性指定标签绑定到哪个表单元素。

当与 [`<output>`](../tags/output.md) 元素一起使用时，`for` 属性指定计算结果与计算中使用的元素之间的关系。

## 适用于

`for` 属性可用于以下元素：

| 元素 Element | 属性 Attribute |
| ----- | ----- |
| [\<label>](../tags/label.md)   | [for](../tags/label_for.md)  |
| [\<output>](../tags/output.md) | [for](../tags/output_for.md) |

## 示例

### For 示例

三个带标签的单选按钮：

```html idoc:preview:iframe
<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form>
```

### Output 示例

执行计算并在 [\<output>](../tags/output.md) 元素中显示结果：

```html idoc:preview:iframe
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
  <input type="range" id="a" value="50">100
  +<input type="number" id="b" value="50">
  =<output name="x" for="a b"></output>
</form>
```

## 浏览器支持

`for` 属性对每个元素都有以下浏览器支持：

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| label   | Yes  | Yes           | Yes | Yes  | Yes  |
| output  | 10.0 | ❌ 不支持| 4.0 | 5.1  | 11.0 |

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg