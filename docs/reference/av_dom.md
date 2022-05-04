HTML Audio/Video DOM 参考
===

HTML5 DOM 具有 [\<audio>](../tags/audio.md) 和 [\<video>](../tags/video.md) 元素的方法、属性和事件。

## HTML Audio/Video 方法

| 方法 Method | 描述 Description |
| ----- | ---- |
| [addTextTrack()](./av/method/addtexttrack.md) | 为音频/视频添加一个新的文本轨道 |
| [canPlayType()](./av/method/canplaytype.md)   | 检查浏览器是否可以播放指定的音频/视频类型 |
| [load()](./av/method/load.md)                 | 重新加载音频/视频元素 |
| [play()](./av/method/play.md)                 | 开始播放音频/视频 |
| [pause()](./av/method/pause.md)               | 暂停当前播放的音频/视频 |
<!--rehype:style=width: 100%; display: inline-table;-->

## HTML Audio/Video 属性

| 属性 Property | 描述 Description |
| ----- | ---- |
| [audioTracks](./av/property/audiotracks.md)                 | 返回表示可用音轨的 AudioTrackList 对象 |
| [autoplay](./av/property/autoplay.md)                       | 设置或返回音频/视频是否应在加载后立即开始播放 |
| [buffered](./av/property/buffered.md)                       | 返回一个 TimeRanges 对象，表示音频/视频的缓冲部分 |
| [controller](./av/property/controller.md)                   | 返回表示当前音频/视频的媒体控制器的 MediaController 对象 |
| [controls](./av/property/controls.md)                       | 设置或返回音频/视频是否应显示控件（如播放/暂停等）。 |
| crossOrigin                                                 | 设置或返回音频/视频的 CORS 设置 |
| [currentSrc](./av/property/currentsrc.md)                   | 返回当前音频/视频的 URL |
| [currentTime](./av/property/currenttime.md)                 | 设置或返回音频/视频中的当前播放位置（以秒为单位） |
| [defaultMuted](./av/property/defaultmuted.md)               | 设置或返回音频/视频是否默认静音 |
| [defaultPlaybackRate](./av/property/defaultplaybackrate.md) | 设置或返回音频/视频播放的默认速度 |
| [duration](./av/property/duration.md)                       | 返回当前音频/视频的长度（以秒为单位） |
| [ended](./av/property/ended.md)                             | 返回音频/视频的播放是否结束 |
| [error](./av/property/error.md)                             | 返回一个 MediaError 对象，表示音频/视频的错误状态 |
| [loop](./av/property/loop.md)                               | 设置或返回音频/视频是否在完成后重新开始 |
| [mediaGroup](./av/property/mediagroup.md)                   | 设置或返回音视频所属的组（用于链接多个音视频元素） |
| [muted](./av/property/muted.md)                             | 设置或返回音频/视频是否静音 |
| [networkState](./av/property/networkstate.md)               | 返回音频/视频的当前网络状态 |
| [paused](./av/property/paused.md)                           | 返回音频/视频是否暂停 |
| [playbackRate](./av/property/playbackrate.md)               | 设置或返回音视频播放速度 |
| [played](./av/property/played.md)                           | 返回代表音频/视频播放部分的 TimeRanges 对象 |
| [preload](./av/property/preload.md)                         | 设置或返回页面加载时是否加载音频/视频 |
| [readyState](./av/property/readystate.md)                   | 返回音频/视频的当前就绪状态 |
| [seekable](./av/property/seekable.md)                       | 返回一个 TimeRanges 对象，表示音频/视频的可搜索部分 |
| [seeking](./av/property/seeking.md)                         | 返回用户当前是否正在寻找音频/视频 |
| [src](./av/property/src.md)                                 | 设置或返回音频/视频元素的当前来源 |
| [startDate](./av/property/startdate.md)                     | 返回表示当前时间偏移量的 Date 对象 |
| [textTracks](./av/property/texttracks.md)                   | 返回一个表示可用文本轨道的 TextTrackList 对象 |
| [videoTracks](./av/property/videotracks.md)                 | 返回一个 VideoTrackList 对象，表示可用的视频轨道 |
| [volume](./av/property/volume.md)                           | 设置或返回音频/视频的音量 |
<!--rehype:style=width: 100%; display: inline-table;-->

## HTML Audio/Video 事件

| 事件 Event | 描述 Description |
| ----- | ---- |
| [abort](./av/event/abort.md)                   | 当音频/视频的加载中止时触发 |
| [canplay](./av/event/canplay.md)               | 当浏览器可以开始播放音频/视频时触发 |
| [canplaythrough](./av/event/canplaythrough.md) | 当浏览器可以播放音频/视频而无需停止缓冲时触发 |
| [durationchange](./av/event/durationchange.md) | 当音频/视频的持续时间改变时触发 |
| emptied                                        | 当前播放列表为空时触发 |
| [ended](./av/event/ended.md)                   | 当前播放列表结束时触发 |
| [error](./av/event/error.md)                   | 在加载音频/视频期间发生错误时触发 |
| [loadeddata](./av/event/loadeddata.md)         | 当浏览器加载音频/视频的当前帧时触发 |
| [loadedmetadata](./av/event/loadedmetadata.md) | 当浏览器加载音频/视频的元数据时触发 |
| [loadstart](./av/event/loadstart.md)           | 当浏览器开始寻找音频/视频时触发 |
| [pause](./av/event/pause.md)                   | 当音频/视频暂停时触发 |
| [play](./av/event/play.md)                     | 当音频/视频已启动或不再暂停时触发 |
| [playing](./av/event/playing.md)               | 在暂停或停止缓冲后播放音频/视频时触发 |
| [progress](./av/event/progress.md)             | 当浏览器下载音频/视频时触发 |
| [ratechange](./av/event/ratechange.md)         | 当音频/视频的播放速度改变时触发 |
| [seeked](./av/event/seeked.md)                 | 当用户完成移动/跳到音频/视频中的新位置时触发 |
| [seeking](./av/event/seeking.md)               | 当用户开始移动/跳到音频/视频中的新位置时触发 |
| [stalled](./av/event/stalled.md)               | 当浏览器尝试获取媒体数据但数据不可用时触发 |
| [suspend](./av/event/suspend.md)               | 当浏览器故意不获取媒体数据时触发 |
| [timeupdate](./av/event/timeupdate.md)         | 当前播放位置改变时触发 |
| [volumechange](./av/event/volumechange.md)     | 当音量改变时触发 |
| [waiting](./av/event/waiting.md)               | 当视频停止时触发，因为它需要缓冲下一帧 |
<!--rehype:style=width: 100%; display: inline-table;-->
