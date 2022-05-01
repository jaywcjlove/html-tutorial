HTML \<picture> 标签
===

## 示例

如何使用 \<picture> 标签：

```html idoc:preview
<picture>
  <source srcset="../assets/example.png" media="(max-width: 600px)">
  <source srcset="../assets/sublime_text.png" media="(max-width: 1500px)">
  <source srcset="../assets/chrome.svg">
  <img src="../assets/example.png" alt="Flowers">
</picture>
```

## 定义和用法

`<picture>` 标签让 Web 开发人员在指定图像资源时更加灵活。

`<picture>` 元素最常用于响应式设计中的艺术指导。 无需根据视口宽度放大或缩小一个图像，而是可以设计多个图像以更好地填充浏览器视口。

`<picture>` 元素包含两个标签：一个或多个 [\<source>](./source.md) 标签和一个 [\<img>](./img.md) 标签。

浏览器将查找媒体查询与当前视口宽度匹配的第一个 [\<source>](./source.md) 元素，然后它将显示正确的图像（在 srcset 属性中指定）。 [\<img>](./img.md) 元素是 `<picture>` 元素的最后一个子元素，如果没有源标签匹配，则作为后备选项。

**提示：** `<picture>` 元素的工作方式与 [\<video>](./video.md) 和 [\<audio>](./audio.md) “相似”。 您设置了不同的来源，第一个符合偏好的来源就是正在使用的来源。

## 浏览器支持

表中的数字指定了完全支持该元素的第一个浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| \<picture> | 38.0 | 13.0 | 38.0 | 9.1 | 25.0 |

## 全局属性

`<picture>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<picture>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。

## 相关页面

HTML 教程: [HTML \<picture> Element](../tutorial/images.md)


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg