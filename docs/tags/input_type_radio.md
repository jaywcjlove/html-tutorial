HTML \<input type="radio">
===

## 示例

单选按钮让用户只选择有限数量的选项之一：

```html idoc:preview:iframe
<input type="radio" id="html" name="fav_language" value="HTML">
<label for="html">HTML</label><br>
<input type="radio" id="css" name="fav_language" value="CSS">
<label for="css">CSS</label><br>
<input type="radio" id="javascript" name="fav_language" value="JavaScript">
<label for="javascript">JavaScript</label>
```

## 定义和用法

`<input type="radio">` 定义了一个单选按钮。

单选按钮通常显示在单选组中（描述一组相关选项的单选按钮的集合）。 一个组中只能同时选择一个单选按钮。

**注意：** 单选组必须具有相同的名称（`name` 属性的值）才能被视为一个组。 创建单选组后，选择该组中的任何单选按钮会自动取消选择同一组中的任何其他选定单选按钮。 只要每个组都有自己的名称，您就可以在一个页面上拥有任意数量的广播组。

**注意：** `value` 属性定义了与每个单选按钮关联的唯一值。 该值不会显示给用户，而是在“提交”时发送到服务器以识别选择了哪个单选按钮的值。

**提示：** 始终添加 `<label>` 标签以获得最佳可访问性实践！

## 浏览器支持

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="radio" | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<input type="radio">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg