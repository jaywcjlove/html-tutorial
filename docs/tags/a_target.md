HTML `<a>` 标签的 target 属性
===

## 示例

`target` 属性指定打开链接文档的位置：

```html idoc:preview
<a target="_blank" href="https://github.com/jaywcjlove/html-tutorial">
  HTML Tutorial
</a>
```

## 定义和用法

`target` 属性指定打开链接文档的位置。

## 浏览器支持

| 属性 | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| target    | Yes | Yes | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<a target="_blank|_self|_parent|_top|framename">
```

## 属性值

| 值 | 描述 |
| ---- | ---- |
| _blank      | 在新窗口或选项卡中打开链接的文档 |
| \_self      | 在单击时在同一框架中打开链接的文档（这是默认设置） |
| \_parent    | 在父框架中打开链接的文档 |
| \_top       | 在整个窗口中打开链接的文档 |
| *framename* | 在命名的 iframe 中打开链接的文档 |
<!--rehype:style=width: 100%; display: inline-table;-->
