HTML \<bdi> 标签
===
## 示例

将用户名与周围的文本方向设置隔离：

```html idoc:preview
<ul>
<li>User <bdi>hrefs</bdi>: 60 points</li>
<li>User <bdi>jdoe</bdi>: 80 points</li>
<li>User <bdi>إيان</bdi>: 90 points</li>
</ul>
```

## 定义和用法

BDI 表示双向隔离(Bi-Directional Isolation)。

`<bdi>` 标记将可能以不同方向格式化的文本部分与它之外的其他文本隔离开。

此元素在嵌入具有未知文本方向的用户生成内容时很有用。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | ---- | ---- | ---- | ---- | ---- |
| \<bdi>  | 16.0 | 79.0 | 10.0 | ❌ 不支持 | 15.0 |


## 全局属性

`<bdi>` 标签支持 HTML 中的[全局属性](../reference/standardattributes.md)。

## 事件属性

`<bdi>` 标签支持 HTML 中的[事件属性](../reference/eventattributes.md)。


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg