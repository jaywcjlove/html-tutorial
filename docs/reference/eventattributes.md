HTML 事件属性
===

## 全局事件属性

HTML 能够让事件触发浏览器中的操作，例如当用户单击元素时启动 JavaScript。

下面是可以添加到 HTML 元素以定义事件操作的全局事件属性。


## Window 事件属性

为 `window` 对象触发的事件（适用于 `<body>` 标签）：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onafterprint](../events/onafterprint.md) | _script_ | 打印文档后运行的脚本 |
| [onbeforeprint](../events/onbeforeprint.md) | _script_ | 在打印文档之前运行的脚本 |
| [onbeforeunload](../events/onbeforeunload.md) | _script_ | 即将卸载文档时运行的脚本 |
| [onerror](../events/onerror.md) | _script_ | 发生错误时要运行的脚本 |
| [onhashchange](../events/onhashchange.md) | _script_ | 当 URL 的锚部分发生更改时运行的脚本 |
| [onload](../events/onload.md) | _script_ | 页面加载完成后触发 |
| onmessage | _script_ | 触发消息时运行的脚本 |
| [onoffline](../events/onoffline.md) | _script_ | 浏览器开始离线工作时运行的脚本 |
| [ononline](../events/ononline.md) | _script_ | 浏览器开始在线工作时运行的脚本 |
| onpagehide | _script_ | 当用户离开页面时运行的脚本 |
| [onpageshow](../events/onpageshow.md) | _script_ | 当用户导航到页面时运行的脚本 |
| onpopstate | _script_ | 窗口历史更改时运行的脚本 |
| [onresize](../events/onresize.md) | _script_ | 调整浏览器窗口大小时触发 |
| onstorage | _script_ | 更新 Web 存储区域时运行的脚本 |
| [onunload](../events/onunload.md) | _script_ | 页面卸载（或浏览器窗口已关闭）时触发 |

## Form 事件

由 HTML 表单中的操作触发的事件（适用于几乎所有 HTML 元素，但最常用于表单元素）：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onblur](../events/onblur.md) | _script_ | 在元素失去焦点时触发 |
| [onchange](../events/onchange.md) | _script_ | 当元素的值改变时触发 |
| [oncontextmenu](../events/oncontextmenu.md) | _script_ | 触发上下文菜单时运行的脚本 |
| [onfocus](../events/onfocus.md) | _script_ | 当元素获得焦点时触发 |
| [oninput](../events/oninput.md) | _script_ | 当元素获得用户输入时运行的脚本 |
| [oninvalid](../events/oninvalid.md) | _script_ | 元素无效时运行的脚本 |
| [onreset](../events/onreset.md) | _script_ | 单击表单中的重置按钮时触发 |
| [onsearch](../events/onsearch.md) | _script_ | 当用户在搜索字段中写入内容时触发 (`<input="search">`) |
| [onselect](../events/onselect.md) | _script_ | 在元素中选择了某些文本后触发 |
| [onsubmit](../events/onsubmit.md) | _script_ | 提交表单时触发 |

## Keyboard 键盘事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onkeydown](../events/onkeydown.md) | _script_ | 当用户按下某个键时触发 |
| [onkeypress](../events/onkeypress.md) | _script_ | 当用户按下某个键时触发 |
| [onkeyup](../events/onkeyup.md) | _script_ | 当用户释放键时触发 |

## Mouse 事件

由鼠标或类似用户动作触发的事件：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onclick](../events/onclick.md) | _script_ | 鼠标点击元素时触发 |
| [ondblclick](../events/ondblclick.md) | _script_ | 鼠标双击元素触发 |
| [onmousedown](../events/onmousedown.md) | _script_ | 在元素上按下鼠标按钮时触发 |
| [onmousemove](../events/onmousemove.md) | _script_ | 当鼠标指针在元素上方移动时触发 |
| [onmouseout](../events/onmouseout.md) | _script_ | 当鼠标指针移出元素时触发 |
| [onmouseover](../events/onmouseover.md) | _script_ | 当鼠标指针移到元素上时触发 |
| [onmouseup](../events/onmouseup.md) | _script_ | 当在元素上释放鼠标按钮时触发 |
| onmousewheel | _script_ | ⚠️ 已弃用。 改用 [onwheel](../events/onwheel.md) 属性 |
| [onwheel](../events/onwheel.md) | _script_ | 当鼠标滚轮在元素上向上或向下滚动时触发 |

## Drag 事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [ondrag](../events/ondrag.md) | _script_ | 拖动元素时运行的脚本 |
| [ondragend](../events/ondragend.md) | _script_ | 在拖动操作结束时运行的脚本 |
| [ondragenter](../events/ondragenter.md) | _script_ | 将元素拖到有效放置目标时运行的脚本 |
| [ondragleave](../events/ondragleave.md) | _script_ | 当元素离开有效放置目标时运行的脚本 |
| [ondragover](../events/ondragover.md) | _script_ | 将元素拖到有效放置目标上时运行的脚本 |
| [ondragstart](../events/ondragstart.md) | _script_ | 在拖动操作开始时运行的脚本 |
| [ondrop](../events/ondrop.md) | _script_ | 拖放拖动元素时运行的脚本 |
| [onscroll](../events/onscroll.md) | _script_ | 滚动元素的滚动条时运行的脚本 |

## Clipboard 事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [oncopy](../events/oncopy.md) | _script_ | 当用户复制元素的内容时触发 |
| [oncut](../events/oncut.md) | _script_ | 当用户剪切元素的内容时触发 |
| [onpaste](../events/onpaste.md) | _script_ | 当用户在元素中粘贴一些内容时触发 |

## 媒体事件

由视频、图像和音频等媒体触发的事件（适用于所有 HTML 元素，但最常见于媒体元素，如 `<audio>`、`<embed>`、`<img>`、`<object>` 和 `<video>`）。

> 提示：查看我们的 [HTML Audio 和 Video DOM 参考](../reference/av_dom.md) 以获取更多信息。

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| onabort | _script_ | 要在中止时运行的脚本 |
| oncanplay | _script_ | 当文件准备好开始播放时运行的脚本（当它缓冲到足以开始播放时） |
| oncanplaythrough | _script_ | 当文件可以一直播放到最后而不暂停缓冲时运行的脚本 |
| oncuechange | _script_ | [\<track>](../tags/track.md) 元素中提示发生变化时运行的脚本 |
| ondurationchange | _script_ | 媒体长度改变时运行的脚本 |
| onemptied | _script_ | 当发生不好的事情并且文件突然不可用（如意外断开连接）时运行的脚本 |
| onended | _script_ | 媒体结束时运行的脚本（对于“感谢收听”等消息的有用事件） |
| onerror | _script_ | 加载文件时发生错误时运行的脚本 |
| onloadeddata | _script_ | 加载媒体数据时运行的脚本 |
| onloadedmetadata | _script_ | 加载元数据（如维度和持续时间）时运行的脚本 |
| onloadstart | _script_ | 在实际加载任何内容之前文件开始加载时运行的脚本 |
| onpause | _script_ | 当媒体被用户或以编程方式暂停时运行的脚本 |
| onplay | _script_ | 媒体准备好开始播放时运行的脚本 |
| onplaying | _script_ | 媒体实际开始播放时运行的脚本 |
| onprogress | _script_ | 当浏览器正在获取媒体数据时运行的脚本 |
| onratechange | _script_ | 每次播放速率变化时运行的脚本（比如当用户切换到慢动作或快进模式时） |
| onseeked | _script_ | 当 seek 属性设置为 false 时要运行的脚本，表示搜索已经结束 |
| onseeking | _script_ | 当 seek 属性设置为 true 时要运行的脚本，表示正在搜索 |
| onstalled | _script_ | 当浏览器由于某种原因无法获取媒体数据时运行的脚本 |
| onsuspend | _script_ | 无论出于何种原因，在完全加载媒体数据之前停止获取媒体数据时运行的脚本 |
| ontimeupdate | _script_ | 当播放位置改变时运行的脚本（比如当用户快进到媒体中的不同点时） |
| onvolumechange | _script_ | 每次更改音量时要运行的脚本（包括将音量设置为`静音 mute`） |
| onwaiting | _script_ | 当媒体暂停但预计会恢复时运行脚本（例如当媒体暂停以缓冲更多数据时） |

## 杂项事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [ontoggle](../events/ontoggle.md) | _script_ | 当用户打开或关闭 [`<details>`](../tags/details.md) 元素时触发 |