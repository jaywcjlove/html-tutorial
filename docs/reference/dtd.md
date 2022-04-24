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
| [&lt;a&gt;](../docs/a.md) | Yes | Yes | Yes |
| [&lt;abbr&gt;](../docs/abbr.md) |Yes | Yes | Yes |
| [&lt;acronym&gt;](../docs/acronym.md) | ❌ | Yes | Yes |
| [&lt;address&gt;](../docs/address.md) |Yes | Yes | Yes |
| [&lt;applet&gt;](../docs/applet.md) | ❌ | Yes | ❌ |
| [&lt;area&gt;](../docs/area.md) |Yes | Yes | ❌ |
| [&lt;article&gt;](../docs/article.md) |Yes | ❌ | ❌ |
| [&lt;aside&gt;](../docs/aside.md) |Yes | ❌ | ❌ |
| [&lt;audio&gt;](../docs/audio.md) |Yes | ❌ | ❌ |
| [&lt;b&gt;](../docs/b.md) |Yes | Yes | Yes |
| [&lt;base&gt;](../docs/base.md) |Yes | Yes | Yes |
| [&lt;basefont&gt;](../docs/basefont.md) | ❌ | Yes | ❌ |
| [&lt;bdi&gt;](../docs/bdi.md) |Yes | ❌ | ❌ |
| [&lt;bdo&gt;](../docs/bdo.md) |Yes | Yes | ❌ |
| [&lt;big&gt;](../docs/big.md) | ❌ | Yes | Yes |
| [&lt;blockquote&gt;](../docs/blockquote.md) |Yes | Yes | Yes |
| [&lt;body&gt;](../docs/body.md) |Yes | Yes | Yes |
| [&lt;br&gt;](../docs/br.md) |Yes | Yes | Yes |
| [&lt;button&gt;](../docs/button.md) |Yes | Yes | Yes |
| [&lt;canvas&gt;](../docs/canvas.md) |Yes | ❌ | ❌ |
| [&lt;caption&gt;](../docs/caption.md) |Yes | Yes | Yes |
| [&lt;center&gt;](../docs/center.md) | ❌ | Yes | ❌ |
| [&lt;cite&gt;](../docs/cite.md) |Yes | Yes | Yes |
| [&lt;code&gt;](../docs/code.md) |Yes | Yes | Yes |
| [&lt;col&gt;](../docs/col.md) |Yes | Yes | ❌ |
| [&lt;colgroup&gt;](../docs/colgroup.md) |Yes | Yes | ❌ |
| [&lt;data&gt;](../docs/data.md) |Yes | ❌ | ❌ |
| [&lt;datalist&gt;](../docs/datalist.md) |Yes | ❌ | ❌ |
| [&lt;dd&gt;](../docs/dd.md) |Yes | Yes | Yes |
| [&lt;del&gt;](../docs/del.md) |Yes | Yes | ❌ |
| [&lt;details&gt;](../docs/details.md) |Yes | ❌ | ❌ |
| [&lt;dfn&gt;](../docs/dfn.md) |Yes | Yes | Yes |
| [&lt;dialog&gt;](../docs/dialog.md) |Yes | ❌ | ❌ |
| [&lt;dir&gt;](../docs/dir.md) | ❌ | Yes | ❌ |
| [&lt;div&gt;](../docs/div.md) |Yes | Yes | Yes |
| [&lt;dl&gt;](../docs/dl.md) |Yes | Yes | Yes |
| [&lt;dt&gt;](../docs/dt.md) |Yes | Yes | Yes |
| [&lt;em&gt;](../docs/em.md) |Yes | Yes | Yes |
| [&lt;embed&gt;](../docs/embed.md) |Yes | ❌ | ❌ |
| [&lt;fieldset&gt;](../docs/fieldset.md) |Yes | Yes | Yes |
| [&lt;figcaption&gt;](../docs/figcaption.md) |Yes | ❌ | ❌ |
| [&lt;figure&gt;](../docs/figure.md) |Yes | ❌ | ❌ |
| [&lt;font&gt;](../docs/font.md) | ❌ | Yes | ❌ |
| [&lt;footer&gt;](../docs/footer.md) |Yes | ❌ | ❌ |
| [&lt;form&gt;](../docs/form.md) |Yes | Yes | Yes |
| [&lt;frame&gt;](../docs/frame.md) | ❌ | ❌ | ❌ |
| [&lt;frameset&gt;](../docs/frameset.md) | ❌ | Yes | ❌ |
| [&lt;h1&gt; to &lt;h6&gt;](../docs/hn.md) |Yes | Yes | Yes |
| [&lt;head&gt;](../docs/head.md) |Yes | Yes | Yes |
| [&lt;header&gt;](../docs/header.md) |Yes | ❌ | ❌ |
| [&lt;hr&gt;](../docs/hr.md) |Yes | Yes | Yes |
| [&lt;html&gt;](../docs/html.md) |Yes | Yes | Yes |
| [&lt;i&gt;](../docs/i.md) |Yes | Yes | Yes |
| [&lt;iframe&gt;](../docs/iframe.md) |Yes | Yes | ❌ |
| [&lt;img&gt;](../docs/img.md) |Yes | Yes | Yes |
| [&lt;input&gt;](../docs/input.md) |Yes | Yes | Yes |
| [&lt;ins&gt;](../docs/ins.md) |Yes | Yes | ❌ |
| [&lt;kbd&gt;](../docs/kbd.md) |Yes | Yes | Yes |
| [&lt;label&gt;](../docs/label.md) |Yes | Yes | Yes |
| [&lt;legend&gt;](../docs/legend.md) |Yes | Yes | Yes |
| [&lt;li&gt;](../docs/li.md) |Yes | Yes | Yes |
| [&lt;link&gt;](../docs/link.md) |Yes | Yes | Yes |
| [&lt;main&gt;](../docs/main.md) |Yes | ❌ | ❌ |
| [&lt;map&gt;](../docs/map.md) |Yes | Yes | ❌ |
| [&lt;mark&gt;](../docs/mark.md) |Yes | ❌ | ❌ |
| [&lt;meta&gt;](../docs/meta.md) |Yes | Yes | Yes |
| [&lt;meter&gt;](../docs/meter.md) |Yes | ❌ | ❌ |
| [&lt;nav&gt;](../docs/nav.md) |Yes | ❌ | ❌ |
| [&lt;noframes&gt;](../docs/noframes.md) | ❌ | Yes | ❌ |
| [&lt;noscript&gt;](../docs/noscript.md) |Yes | Yes | Yes |
| [&lt;object&gt;](../docs/object.md) |Yes | Yes | Yes |
| [&lt;ol&gt;](../docs/ol.md) |Yes | Yes | Yes |
| [&lt;optgroup&gt;](../docs/optgroup.md) |Yes | Yes | Yes |
| [&lt;option&gt;](../docs/option.md) |Yes | Yes | Yes |
| [&lt;output&gt;](../docs/output.md) |Yes | ❌ | ❌ |
| [&lt;p&gt;](../docs/p.md) |Yes | Yes | Yes |
| [&lt;param&gt;](../docs/param.md) |Yes | Yes | Yes |
| [&lt;picture&gt;](../docs/picture.md) |Yes | ❌ | ❌ |
| [&lt;pre&gt;](../docs/pre.md) |Yes | Yes | Yes |
| [&lt;progress&gt;](../docs/progress.md) |Yes | ❌ | ❌ |
| [&lt;q&gt;](../docs/q.md) |Yes | Yes | Yes |
| [&lt;rp&gt;](../docs/rp.md) |Yes | ❌ | ❌ |
| [&lt;rt&gt;](../docs/rt.md) |Yes | ❌ | ❌ |
| [&lt;ruby&gt;](../docs/ruby.md) |Yes | ❌ | ❌ |
| [&lt;s&gt;](../docs/s.md) |Yes | Yes | ❌ |
| [&lt;samp&gt;](../docs/samp.md) |Yes | Yes | Yes |
| [&lt;script&gt;](../docs/script.md) |Yes | Yes | Yes |
| [&lt;section&gt;](../docs/section.md) |Yes | ❌ | ❌ |
| [&lt;select&gt;](../docs/select.md) |Yes | Yes | Yes |
| [&lt;small&gt;](../docs/small.md) |Yes | Yes | Yes |
| [&lt;source&gt;](../docs/source.md) |Yes | ❌ | ❌ |
| [&lt;span&gt;](../docs/span.md) |Yes | Yes | Yes |
| [&lt;strike&gt;](../docs/strike.md) | ❌ | Yes | ❌ |
| [&lt;strong&gt;](../docs/strong.md) |Yes | Yes | Yes |
| [&lt;style&gt;](../docs/style.md) |Yes | Yes | Yes |
| [&lt;sub&gt;](../docs/sub.md) |Yes | Yes | Yes |
| [&lt;summary&gt;](../docs/summary.md) |Yes | ❌ | ❌ |
| [&lt;sup&gt;](../docs/sup.md) |Yes | Yes | Yes |
| [&lt;table&gt;](../docs/table.md) |Yes | Yes | Yes |
| [&lt;tbody&gt;](../docs/tbody.md) |Yes | Yes | ❌ |
| [&lt;td&gt;](../docs/td.md) |Yes | Yes | Yes |
| [&lt;template&gt;](../docs/template.md) |Yes | ❌ | ❌ |
| [&lt;textarea&gt;](../docs/textarea.md) |Yes | Yes | Yes |
| [&lt;tfoot&gt;](../docs/tfoot.md) |Yes | Yes | ❌ |
| [&lt;th&gt;](../docs/th.md) |Yes | Yes | Yes |
| [&lt;thead&gt;](../docs/thead.md) |Yes | Yes | ❌ |
| [&lt;time&gt;](../docs/time.md) |Yes | ❌ | ❌ |
| [&lt;title&gt;](../docs/title.md) |Yes | Yes | Yes |
| [&lt;tr&gt;](../docs/tr.md) |Yes | Yes | Yes |
| [&lt;track&gt;](../docs/track.md) |Yes | ❌ | ❌ |
| [&lt;tt&gt;](../docs/tt.md) | ❌ | Yes | Yes |
| [&lt;u&gt;](../docs/u.md) |Yes | Yes | ❌ |
| [&lt;ul&gt;](../docs/ul.md) |Yes | Yes | Yes |
| [&lt;var&gt;](../docs/var.md) |Yes | Yes | Yes |
| [&lt;video&gt;](../docs/video.md) |Yes | ❌ | ❌ |
| [&lt;wbr&gt;](../docs/wbr.md) |Yes | ❌ | ❌ |