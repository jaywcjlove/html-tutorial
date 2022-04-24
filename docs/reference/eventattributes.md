HTML 事件属性
===

## 全局事件属性

HTML 能够让事件触发浏览器中的操作，例如当用户单击元素时启动 JavaScript。

下面是可以添加到 HTML 元素以定义事件操作的全局事件属性。


## Window 事件属性

为 `window` 对象触发的事件（适用于 `<body>` 标签）：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onafterprint](../events/onafterprint.md) | script | Script to be run after the document is printed |
| [onbeforeprint](../events/onbeforeprint.md) | script | Script to be run before the document is printed |
| [onbeforeunload](../events/onbeforeunload.md) | script | Script to be run when the document is about to be unloaded |
| [onerror](../events/onerror.md) | script | Script to be run when an error occurs |
| [onhashchange](../events/onhashchange.md) | script | Script to be run when there has been changes to the anchor part of the a URL |
| [onload](../events/onload.md) | script | Fires after the page is finished loading |
| onmessage | script | Script to be run when the message is triggered |
| [onoffline](../events/onoffline.md) | script | Script to be run when the browser starts to work offline |
| [ononline](../events/ononline.md) | script | Script to be run when the browser starts to work online |
| onpagehide | script | Script to be run when a user navigates away from a page |
| [onpageshow](../events/onpageshow.md) | script | Script to be run when a user navigates to a page |
| onpopstate | script | Script to be run when the window's history changes |
| [onresize](../events/onresize.md) | script | Fires when the browser window is resized |
| onstorage | script | Script to be run when a Web Storage area is updated |
| [onunload](../events/onunload.md) | script | Fires once a page has unloaded (or the browser window has been closed) |

## Form 事件

由 HTML 表单中的操作触发的事件（适用于几乎所有 HTML 元素，但最常用于表单元素）：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onblur](../events/onblur.md) | _script_ | Fires the moment that the element loses focus |
| [onchange](../events/onchange.md) | _script_ | Fires the moment when the value of the element is changed |
| [oncontextmenu](../events/oncontextmenu.md) | _script_ | Script to be run when a context menu is triggered |
| [onfocus](../events/onfocus.md) | _script_ | Fires the moment when the element gets focus |
| [oninput](../events/oninput.md) | _script_ | Script to be run when an element gets user input |
| [oninvalid](../events/oninvalid.md) | _script_ | Script to be run when an element is invalid |
| [onreset](../events/onreset.md) | _script_ | Fires when the Reset button in a form is clicked |
| [onsearch](../events/onsearch.md) | _script_ | Fires when the user writes something in a search field (&lt;input="search"&gt;) |
| [onselect](../events/onselect.md) | _script_ | Fires after some text has been selected in an element |
| [onsubmit](../events/onsubmit.md) | _script_ | Fires when a form is submitted |

## Keyboard 键盘事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onkeydown](../events/onkeydown.md) | _script_ | Fires when a user is pressing a key |
| [onkeypress](../events/onkeypress.md) | _script_ | Fires when a user presses a key |
| [onkeyup](../events/onkeyup.md) | _script_ | Fires when a user releases a key |

## Mouse 事件

由鼠标或类似用户动作触发的事件：

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [onclick](../events/onclick.md) | _script_ | Fires on a mouse click on the element |
| [ondblclick](../events/ondblclick.md) | _script_ | Fires on a mouse double-click on the element |
| [onmousedown](../events/onmousedown.md) | _script_ | Fires when a mouse button is pressed down on an element |
| [onmousemove](../events/onmousemove.md) | _script_ | Fires when the mouse pointer is moving while it is over an element |
| [onmouseout](../events/onmouseout.md) | _script_ | Fires when the mouse pointer moves out of an element |
| [onmouseover](../events/onmouseover.md) | _script_ | Fires when the mouse pointer moves over an element |
| [onmouseup](../events/onmouseup.md) | _script_ | Fires when a mouse button is released over an element |
| onmousewheel | _script_ |  Deprecated. Use the [onwheel](../events/onwheel.md) attribute instead |
| [onwheel](../events/onwheel.md) | _script_ | Fires when the mouse wheel rolls up or down over an element |

## Drag 事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [ondrag](../events/ondrag.md) | _script_ | Script to be run when an element is dragged |
| [ondragend](../events/ondragend.md) | _script_ | Script to be run at the end of a drag operation |
| [ondragenter](../events/ondragenter.md) | _script_ | Script to be run when an element has been dragged to a valid drop target |
| [ondragleave](../events/ondragleave.md) | _script_ | Script to be run when an element leaves a valid drop target |
| [ondragover](../events/ondragover.md) | _script_ | Script to be run when an element is being dragged over a valid drop target |
| [ondragstart](../events/ondragstart.md) | _script_ | Script to be run at the start of a drag operation |
| [ondrop](../events/ondrop.md) | _script_ | Script to be run when dragged element is being dropped |
| [onscroll](../events/onscroll.md) | _script_ | Script to be run when an element's scrollbar is being scrolled |

## Clipboard 事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [oncopy](../events/oncopy.md) | _script_ | Fires when the user copies the content of an element |
| [oncut](../events/oncut.md) | _script_ | Fires when the user cuts the content of an element |
| [onpaste](../events/onpaste.md) | _script_ | Fires when the user pastes some content in an element |

## 媒体事件

由视频、图像和音频等媒体触发的事件（适用于所有 HTML 元素，但最常见于媒体元素，如 `<audio>`、`<embed>`、`<img>`、`<object>` 和 `<video>`）。

> 提示：查看我们的 [HTML Audio 和 Video DOM 参考](../reference/av_dom.md) 以获取更多信息。

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| onabort | _script_ | Script to be run on abort |
| oncanplay | _script_ | Script to be run when a file is ready to start playing (when it has buffered enough to begin) |
| oncanplaythrough | _script_ | Script to be run when a file can be played all the way to the end without pausing for buffering |
| oncuechange | _script_ | Script to be run when the cue changes in a &lt;track&gt; element |
| ondurationchange | _script_ | Script to be run when the length of the media changes |
| onemptied | _script_ | Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects) |
| onended | _script_ | Script to be run when the media has reach the end (a useful event for messages like "thanks for listening") |
| onerror | _script_ | Script to be run when an error occurs when the file is being loaded  |
| onloadeddata | _script_ | Script to be run when media data is loaded |
| onloadedmetadata | _script_ | Script to be run when meta data (like dimensions and duration) are loaded |
| onloadstart | _script_ | Script to be run just as the file begins to load before anything is actually loaded |
| onpause | _script_ | Script to be run when the media is paused either by the user or programmatically |
| onplay | _script_ | Script to be run when the media is ready to start playing |
| onplaying | _script_ | Script to be run when the media actually has started playing |
| onprogress | _script_ | Script to be run when the browser is in the process of getting the media data |
| onratechange | _script_ | Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode) |
| onseeked | _script_ | Script to be run when the seeking attribute is set to false indicating that seeking has ended |
| onseeking | _script_ | Script to be run when the seeking attribute is set to true indicating that seeking is active |
| onstalled | _script_ | Script to be run when the browser is unable to fetch the media data for whatever reason |
| onsuspend | _script_ | Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason |
| ontimeupdate | _script_ | Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media) |
| onvolumechange | _script_ | Script to be run each time the volume is changed which (includes setting the volume to "mute") |
| onwaiting | _script_ | Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data) |

## 杂项事件

| 属性 Attribute | Value | 描述 Description |
| ---- | ---- | ---- |
| [ontoggle](../events/ontoggle.md) | script | Fires when the user opens or closes the `<details>` element |