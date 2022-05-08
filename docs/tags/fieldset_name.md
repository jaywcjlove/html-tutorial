HTML \<fieldset> name 属性
===

## 示例

具有 name 属性的 \<fieldset>：

```html idoc:preview:iframe
<form action="/action_page.php" method="get">
  <fieldset name="personalia">
    <label for="fname">名:</label>
    <input type="text" id="fname" name="fname">
  </fieldset>
  <br>
  <button type="button"
  onclick="form.personalia.style.backgroundColor='yellow'">
  更改字段集的背景颜色</button>
  <input type="submit">
</form>
```

## 定义和用法

`name` 属性指定字段集的名称。

`name` 属性用于引用 JavaScript 中的元素，或在提交表单后引用表单数据。

## 浏览器支持

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| name      | Yes | 11.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<fieldset name="*text*">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| *name* | 指定字段集的名称 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
