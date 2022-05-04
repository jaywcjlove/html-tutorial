HTML `<!DOCTYPE>`
===

## HTML 文档类型

所有 HTML 文档都必须以 `<!DOCTYPE>` 声明开头。

声明不是 HTML 标记。 对于浏览器来说，这是一个关于预期文档类型的“信息”。

在 HTML5 中，`<!DOCTYPE>` 声明很简单：

```html
<!DOCTYPE html>
```

在旧文档（HTML 4 或 XHTML）中，声明更复杂，因为声明必须引用 DTD（文档类型定义）。

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```

您可以在 [<!DOCTYPE>](../tags/doctype.md) 参考中阅读有关文档类型的更多信息。


## 不同 DOCTYPES 中的有效 HTML 元素


| Tag | HTML 5 | HTML 4 | XHTML |
| ---- | ---- | ---- | ---- |
| [&lt;a&gt;](../tags/a.md) | Yes | Yes | Yes |
| [&lt;abbr&gt;](../tags/abbr.md) |Yes | Yes | Yes |
| [&lt;acronym&gt;](../tags/acronym.md) | ❌ | Yes | Yes |
| [&lt;address&gt;](../tags/address.md) |Yes | Yes | Yes |
| [&lt;applet&gt;](../tags/applet.md) | ❌ | Yes | ❌ |
| [&lt;area&gt;](../tags/area.md) |Yes | Yes | ❌ |
| [&lt;article&gt;](../tags/article.md) |Yes | ❌ | ❌ |
| [&lt;aside&gt;](../tags/aside.md) |Yes | ❌ | ❌ |
| [&lt;audio&gt;](../tags/audio.md) |Yes | ❌ | ❌ |
| [&lt;b&gt;](../tags/b.md) |Yes | Yes | Yes |
| [&lt;base&gt;](../tags/base.md) |Yes | Yes | Yes |
| [&lt;basefont&gt;](../tags/basefont.md) | ❌ | Yes | ❌ |
| [&lt;bdi&gt;](../tags/bdi.md) |Yes | ❌ | ❌ |
| [&lt;bdo&gt;](../tags/bdo.md) |Yes | Yes | ❌ |
| [&lt;big&gt;](../tags/big.md) | ❌ | Yes | Yes |
| [&lt;blockquote&gt;](../tags/blockquote.md) |Yes | Yes | Yes |
| [&lt;body&gt;](../tags/body.md) |Yes | Yes | Yes |
| [&lt;br&gt;](../tags/br.md) |Yes | Yes | Yes |
| [&lt;button&gt;](../tags/button.md) |Yes | Yes | Yes |
| [&lt;canvas&gt;](../tags/canvas.md) |Yes | ❌ | ❌ |
| [&lt;caption&gt;](../tags/caption.md) |Yes | Yes | Yes |
| [&lt;center&gt;](../tags/center.md) | ❌ | Yes | ❌ |
| [&lt;cite&gt;](../tags/cite.md) |Yes | Yes | Yes |
| [&lt;code&gt;](../tags/code.md) |Yes | Yes | Yes |
| [&lt;col&gt;](../tags/col.md) |Yes | Yes | ❌ |
| [&lt;colgroup&gt;](../tags/colgroup.md) |Yes | Yes | ❌ |
| [&lt;data&gt;](../tags/data.md) |Yes | ❌ | ❌ |
| [&lt;datalist&gt;](../tags/datalist.md) |Yes | ❌ | ❌ |
| [&lt;dd&gt;](../tags/dd.md) |Yes | Yes | Yes |
| [&lt;del&gt;](../tags/del.md) |Yes | Yes | ❌ |
| [&lt;details&gt;](../tags/details.md) |Yes | ❌ | ❌ |
| [&lt;dfn&gt;](../tags/dfn.md) |Yes | Yes | Yes |
| [&lt;dialog&gt;](../tags/dialog.md) |Yes | ❌ | ❌ |
| [&lt;dir&gt;](../tags/dir.md) | ❌ | Yes | ❌ |
| [&lt;div&gt;](../tags/div.md) |Yes | Yes | Yes |
| [&lt;dl&gt;](../tags/dl.md) |Yes | Yes | Yes |
| [&lt;dt&gt;](../tags/dt.md) |Yes | Yes | Yes |
| [&lt;em&gt;](../tags/em.md) |Yes | Yes | Yes |
| [&lt;embed&gt;](../tags/embed.md) |Yes | ❌ | ❌ |
| [&lt;fieldset&gt;](../tags/fieldset.md) |Yes | Yes | Yes |
| [&lt;figcaption&gt;](../tags/figcaption.md) |Yes | ❌ | ❌ |
| [&lt;figure&gt;](../tags/figure.md) |Yes | ❌ | ❌ |
| [&lt;font&gt;](../tags/font.md) | ❌ | Yes | ❌ |
| [&lt;footer&gt;](../tags/footer.md) |Yes | ❌ | ❌ |
| [&lt;form&gt;](../tags/form.md) |Yes | Yes | Yes |
| [&lt;frame&gt;](../tags/frame.md) | ❌ | ❌ | ❌ |
| [&lt;frameset&gt;](../tags/frameset.md) | ❌ | Yes | ❌ |
| [&lt;h1&gt; to &lt;h6&gt;](../tags/hn.md) |Yes | Yes | Yes |
| [&lt;head&gt;](../tags/head.md) |Yes | Yes | Yes |
| [&lt;header&gt;](../tags/header.md) |Yes | ❌ | ❌ |
| [&lt;hr&gt;](../tags/hr.md) |Yes | Yes | Yes |
| [&lt;html&gt;](../tags/html.md) |Yes | Yes | Yes |
| [&lt;i&gt;](../tags/i.md) |Yes | Yes | Yes |
| [&lt;iframe&gt;](../tags/iframe.md) |Yes | Yes | ❌ |
| [&lt;img&gt;](../tags/img.md) |Yes | Yes | Yes |
| [&lt;input&gt;](../tags/input.md) |Yes | Yes | Yes |
| [&lt;ins&gt;](../tags/ins.md) |Yes | Yes | ❌ |
| [&lt;kbd&gt;](../tags/kbd.md) |Yes | Yes | Yes |
| [&lt;label&gt;](../tags/label.md) |Yes | Yes | Yes |
| [&lt;legend&gt;](../tags/legend.md) |Yes | Yes | Yes |
| [&lt;li&gt;](../tags/li.md) |Yes | Yes | Yes |
| [&lt;link&gt;](../tags/link.md) |Yes | Yes | Yes |
| [&lt;main&gt;](../tags/main.md) |Yes | ❌ | ❌ |
| [&lt;map&gt;](../tags/map.md) |Yes | Yes | ❌ |
| [&lt;mark&gt;](../tags/mark.md) |Yes | ❌ | ❌ |
| [&lt;meta&gt;](../tags/meta.md) |Yes | Yes | Yes |
| [&lt;meter&gt;](../tags/meter.md) |Yes | ❌ | ❌ |
| [&lt;nav&gt;](../tags/nav.md) |Yes | ❌ | ❌ |
| [&lt;noframes&gt;](../tags/noframes.md) | ❌ | Yes | ❌ |
| [&lt;noscript&gt;](../tags/noscript.md) |Yes | Yes | Yes |
| [&lt;object&gt;](../tags/object.md) |Yes | Yes | Yes |
| [&lt;ol&gt;](../tags/ol.md) |Yes | Yes | Yes |
| [&lt;optgroup&gt;](../tags/optgroup.md) |Yes | Yes | Yes |
| [&lt;option&gt;](../tags/option.md) |Yes | Yes | Yes |
| [&lt;output&gt;](../tags/output.md) |Yes | ❌ | ❌ |
| [&lt;p&gt;](../tags/p.md) |Yes | Yes | Yes |
| [&lt;param&gt;](../tags/param.md) |Yes | Yes | Yes |
| [&lt;picture&gt;](../tags/picture.md) |Yes | ❌ | ❌ |
| [&lt;pre&gt;](../tags/pre.md) |Yes | Yes | Yes |
| [&lt;progress&gt;](../tags/progress.md) |Yes | ❌ | ❌ |
| [&lt;q&gt;](../tags/q.md) |Yes | Yes | Yes |
| [&lt;rp&gt;](../tags/rp.md) |Yes | ❌ | ❌ |
| [&lt;rt&gt;](../tags/rt.md) |Yes | ❌ | ❌ |
| [&lt;ruby&gt;](../tags/ruby.md) |Yes | ❌ | ❌ |
| [&lt;s&gt;](../tags/s.md) |Yes | Yes | ❌ |
| [&lt;samp&gt;](../tags/samp.md) |Yes | Yes | Yes |
| [&lt;script&gt;](../tags/script.md) |Yes | Yes | Yes |
| [&lt;section&gt;](../tags/section.md) |Yes | ❌ | ❌ |
| [&lt;select&gt;](../tags/select.md) |Yes | Yes | Yes |
| [&lt;small&gt;](../tags/small.md) |Yes | Yes | Yes |
| [&lt;source&gt;](../tags/source.md) |Yes | ❌ | ❌ |
| [&lt;span&gt;](../tags/span.md) |Yes | Yes | Yes |
| [&lt;strike&gt;](../tags/strike.md) | ❌ | Yes | ❌ |
| [&lt;strong&gt;](../tags/strong.md) |Yes | Yes | Yes |
| [&lt;style&gt;](../tags/style.md) |Yes | Yes | Yes |
| [&lt;sub&gt;](../tags/sub.md) |Yes | Yes | Yes |
| [&lt;summary&gt;](../tags/summary.md) |Yes | ❌ | ❌ |
| [&lt;sup&gt;](../tags/sup.md) |Yes | Yes | Yes |
| [&lt;table&gt;](../tags/table.md) |Yes | Yes | Yes |
| [&lt;tbody&gt;](../tags/tbody.md) |Yes | Yes | ❌ |
| [&lt;td&gt;](../tags/td.md) |Yes | Yes | Yes |
| [&lt;template&gt;](../tags/template.md) |Yes | ❌ | ❌ |
| [&lt;textarea&gt;](../tags/textarea.md) |Yes | Yes | Yes |
| [&lt;tfoot&gt;](../tags/tfoot.md) |Yes | Yes | ❌ |
| [&lt;th&gt;](../tags/th.md) |Yes | Yes | Yes |
| [&lt;thead&gt;](../tags/thead.md) |Yes | Yes | ❌ |
| [&lt;time&gt;](../tags/time.md) |Yes | ❌ | ❌ |
| [&lt;title&gt;](../tags/title.md) |Yes | Yes | Yes |
| [&lt;tr&gt;](../tags/tr.md) |Yes | Yes | Yes |
| [&lt;track&gt;](../tags/track.md) |Yes | ❌ | ❌ |
| [&lt;tt&gt;](../tags/tt.md) | ❌ | Yes | Yes |
| [&lt;u&gt;](../tags/u.md) |Yes | Yes | ❌ |
| [&lt;ul&gt;](../tags/ul.md) |Yes | Yes | Yes |
| [&lt;var&gt;](../tags/var.md) |Yes | Yes | Yes |
| [&lt;video&gt;](../tags/video.md) |Yes | ❌ | ❌ |
| [&lt;wbr&gt;](../tags/wbr.md) |Yes | ❌ | ❌ |
<!--rehype:style=width: 100%; display: inline-table;-->