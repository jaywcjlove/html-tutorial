HTML Canvas 参考
===

HTML [`<canvas>`](../tags/canvas.md) 标签用于通过脚本（通常是 JavaScript）动态绘制图形。

## 颜色、样式和阴影

| 属性 | 描述 |
| ---- | ---- |
| [fillStyle](../tags/canvas_fillstyle.md) | 设置或返回用于填充绘画的颜色、渐变或模式 |
| [strokeStyle](../tags/canvas_strokestyle.md) | 设置或返回用于笔触的颜色、渐变或模式 |
| [shadowColor](../tags/canvas_shadowcolor.md) | 设置或返回用于阴影的颜色 |
| [shadowBlur](../tags/canvas_shadowblur.md) | 设置或返回用于阴影的模糊级别 |
| [shadowOffsetX](../tags/canvas_shadowoffsetx.md) | 设置或返回阴影距形状的水平距离 |
| [shadowOffsetY](../tags/canvas_shadowoffsety.md) | 设置或返回阴影距形状的垂直距离 |
<!--rehype:style=width: 100%; display: inline-table;-->

| 方法 | 描述 |
| ---- | ---- |
| [createLinearGradient()](../tags/canvas_createlineargradient.md) | 创建线性渐变（用在画布内容上） |
| [createPattern()](../tags/canvas_createpattern.md) | 在指定的方向上重复指定的元素 |
| [createRadialGradient()](../tags/canvas_createradialgradient.md) | 创建放射状/环形的渐变（用在画布内容上） |
| [addColorStop()](../tags/canvas_addcolorstop.md) | 规定渐变对象中的颜色和停止位置 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 线条样式(Line Styles)

| 属性 | 描述 |
| ---- | ---- |
| [lineCap](../tags/canvas_linecap.md) | 设置或返回线条的结束端点样式 |
| [lineJoin](../tags/canvas_linejoin.md) | 设置或返回两条线相交时，所创建的拐角类型 |
| [lineWidth](../tags/canvas_linewidth.md) | 设置或返回当前的线条宽度 |
| [miterLimit](../tags/canvas_miterlimit.md) | 设置或返回最大斜接长度 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 矩形(Rectangles)

| 方法 | 描述 |
| ---- | ---- |
| [rect()](../tags/canvas_rect.md) | 创建矩形 |
| [fillRect()](../tags/canvas_fillrect.md) | 绘制“被填充”的矩形 |
| [strokeRect()](../tags/canvas_strokerect.md) | 绘制矩形（无填充） |
| [clearRect()](../tags/canvas_clearrect.md) | 在给定的矩形内清除指定的像素 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 路径(Paths)

| 方法 | 描述 |
| ---- | ---- |
| [fill()](../tags/canvas_fill.md) | 填充当前绘图（路径） |
| [stroke()](../tags/canvas_stroke.md) | 绘制已定义的路径 |
| [beginPath()](../tags/canvas_beginpath.md) | 起始一条路径，或重置当前路径 |
| [moveTo()](../tags/canvas_moveto.md) | 把路径移动到画布中的指定点，不创建线条 |
| [closePath()](../tags/canvas_closepath.md) | 创建从当前点回到起始点的路径 |
| [lineTo()](../tags/canvas_lineto.md) | 添加一个新点，然后在画布中创建从该点到最后指定点的线条 |
| [clip()](../tags/canvas_clip.md) | 从原始画布剪切任意形状和尺寸的区域 |
| [quadraticCurveTo()](../tags/canvas_quadraticcurveto.md) | 创建二次贝塞尔曲线 |
| [bezierCurveTo()](../tags/canvas_beziercurveto.md) | 创建三次方贝塞尔曲线 |
| [arc()](../tags/canvas_arc.md) | 创建弧/曲线（用于创建圆形或部分圆） |
| [arcTo()](../tags/canvas_arcto.md) | 创建两切线之间的弧/曲线 |
| [isPointInPath()](../tags/canvas_ispointinpath.md) | 如果指定的点位于当前路径中，则返回 true，否则返回 false |
<!--rehype:style=width: 100%; display: inline-table;-->

## 转换(Transformations)

| 方法 | 描述 |
| ---- | ---- |
| [scale()](../tags/canvas_scale.md) | 缩放当前绘图至更大或更小 |
| [rotate()](../tags/canvas_rotate.md) | 旋转当前绘图 |
| [translate()](../tags/canvas_translate.md) | 重新映射画布上的 (0,0) 位置 |
| [transform()](../tags/canvas_transform.md) | 替换绘图的当前转换矩阵 |
| [setTransform()](../tags/canvas_settransform.md) | 将当前转换重置为单位矩阵。然后运行 transform() |
<!--rehype:style=width: 100%; display: inline-table;-->

## 文本(Text)

| 属性 | 描述 |
| ---- | ---- |
| [font](../tags/canvas_font.md) | 设置或返回文本内容的当前字体属性 |
| [textAlign](../tags/canvas_textalign.md) | 设置或返回文本内容的当前对齐方式 |
| [textBaseline](../tags/canvas_textbaseline.md) | 设置或返回在绘制文本时使用的当前文本基线 |
<!--rehype:style=width: 100%; display: inline-table;-->

| 方法 | 描述 |
| ---- | ---- |
| [fillText()](../tags/canvas_filltext.md) | 在画布上绘制“被填充的”文本 |
| [strokeText()](../tags/canvas_stroketext.md) | 在画布上绘制文本（无填充） |
| [measureText()](../tags/canvas_measuretext.md) | 返回包含指定文本宽度的对象 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 图像绘制(Image Drawing)

| 方法 | 描述 |
| ---- | ---- |
| [drawImage()](../tags/canvas_drawimage.md) | 向画布上绘制图像、画布或视频 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 像素操作(Pixel Manipulation)

| 属性 | 描述 |
| ---- | ---- |
| [width](../tags/canvas_imagedata_width.md) | 返回 ImageData 对象的宽度 |
| [height](../tags/canvas_imagedata_height.md) | 返回 ImageData 对象的高度 |
| [data](../tags/canvas_imagedata_data.md) | 返回一个对象，其包含指定的 ImageData 对象的图像数据 |
<!--rehype:style=width: 100%; display: inline-table;-->

| 方法 | 描述 |
| ---- | ---- |
| [createImageData()](../tags/canvas_createimagedata.md) | 创建新的、空白的 ImageData 对象 |
| [getImageData()](../tags/canvas_getimagedata.md) | 返回 ImageData 对象，该对象为画布上指定的矩形复制像素数据 |
| [putImageData()](../tags/canvas_putimagedata.md) | 把图像数据（从指定的 ImageData 对象）放回画布上 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 合成(Compositing)

| 属性 | 描述 |
| ---- | ---- |
| [globalAlpha](../tags/canvas_globalalpha.md) | 设置或返回绘图的当前 alpha 或透明值 |
| [globalCompositeOperation](../tags/canvas_globalcompositeoperation.md) | 设置或返回新图像如何绘制到已有的图像上 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 其他(Other)

| 方法 | 描述 |
| ---- | ---- |
| save() | 保存当前环境的状态 |
| restore() | 返回之前保存过的路径状态和属性 |
| createEvent() |   |
| getContext() |   |
| toDataURL() |   |
<!--rehype:style=width: 100%; display: inline-table;-->