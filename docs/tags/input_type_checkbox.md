HTML \<input type="checkbox">
===

## 示例

让用户从有限数量的选项中选择一个或多个选项：

```html idoc:preview:iframe
<input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
<label for="vehicle1"> I have a bike</label><br>
<input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
<label for="vehicle2"> I have a car</label><br>
<input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
<label for="vehicle3"> I have a boat</label><br>
```

## 定义和用法

`<input type="checkbox">` 定义了一个复选框。

复选框显示为一个方框，激活时勾选（选中）。

复选框用于让用户从有限数量的选项中选择一个或多个选项。

**提示：** 始终添加 [`<label>`](./label.md) 标签以获得最佳可访问性实践！

## 浏览器支持

| Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type="checkbox" | Yes | Yes | Yes | Yes | Yes |


## 语法

```html
<input type="checkbox">
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg