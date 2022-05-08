HTML \<iframe> sandbox 属性
===

## 示例

具有额外限制的 \<iframe>：

```html idoc:preview:iframe
<iframe
  src="iframe.html"
  sandbox
>

</iframe>
```

## 定义和用法

`sandbox` 属性为 iframe 中的内容启用了一组额外的限制。

当 `sandbox` 属性存在时，它将：

* 将内容视为来自一个独特的来源
* 阻止表单提交
* 阻止脚本执行
* 禁用 API
* 防止链接针对其他浏览上下文
* 防止内容使用插件（通过 `<embed>`、`<object>`、`<applet>` 或其他）
* 阻止内容导航其顶级浏览上下文
* 阻止自动触发的功能（例如自动播放视频或自动聚焦表单控件）

`sandbox` 属性的值可以是空的（然后应用所有限制），也可以是空格分隔的预定义值列表，这些值将删除特定限制。

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 属性 Attribute | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| sandbox   | 4.0 | 10.0 | 17.0 | 5.0 | 15.0 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 语法

```html
<iframe sandbox="value">
```

## 属性值

| 值 Value | 描述 Description |
| ----- | ----- |
| (*no value*)                            | 应用所有限制 |
| allow-forms                             | 允许表单提交 |
| allow-modals                            | 允许打开模态窗口 |
| allow-orientation-lock                  | 允许锁定屏幕方向 |
| allow-pointer-lock                      | 允许使用指针锁定 API |
| allow-popups                            | 允许弹出窗口 |
| allow-popups-to-escape-sandbox          | 允许弹出窗口在不继承沙盒的情况下打开新窗口 |
| allow-presentation                      | 允许开始演示会话 |
| allow-same-origin                       | 允许将 iframe 内容视为来自同一来源 |
| allow-scripts                           | 允许运行脚本 |
| allow-top-navigation                    | 允许 iframe 内容导航其顶级浏览上下文 |
| allow-top-navigation-by-user-activation | 允许 iframe 内容导航其顶级浏览上下文，但前提是由用户启动 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

允许表单提交的 \<iframe> 沙箱：

```html idoc:preview:iframe
<iframe
  src="form.html"
  sandbox="allow-forms"
>
</iframe>
```

允许脚本的 \<iframe> 沙箱：

```html idoc:preview:iframe
<iframe
  src="script.html"
  sandbox="allow-scripts"
>
</iframe>
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg

