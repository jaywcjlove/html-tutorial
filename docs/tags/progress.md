HTML \<progress> Tag
===

## 示例

显示进度条：

```html idoc:preview
<label for="file">下载进度：</label>
<progress id="file" value="32" max="100"> 32% </progress>
```

## 定义和用法

`<progress>` 标签表示任务的完成进度。

**提示：** 始终添加 [\<label>](./label.md) 标记以获得最佳可访问性实践！

## 提示和注意事项

**提示：** 结合 JavaScript 使用 `<progress>` 标签来显示任务的进度。

**注意**：`<progress>` 标签不适合表示量表（例如磁盘空间使用情况或查询结果的相关性）。 要表示仪表，请改用 [\<meter>](./meter.md) 标记。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<progress> | 8.0 | 10.0 | 16.0 | 6.0 | 11.0 |

## 属性 Attributes

| 属性 | 值 | 描述 |
| ---- | ---- | ---- |
| [max](./progress_max.md)     | *number* | 指定任务总共需要多少工作。 默认值为 1 |
| [value](./progress_value.md) | *number* | 指定已完成多少任务 |

## 全局属性

`<progress>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<progress>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg