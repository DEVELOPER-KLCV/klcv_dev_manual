---
layout: default

grand_parent: TabFrame Class
parent: Properties
has_children: false
title: TabFrame.Arrangement Property
nav_order: 1
permalink: /package/extension3/tabframe/properties/arrangement
---
# {{ page.title }}
<br>

Set how to arrange tabs.

| Constant     | Value | Description                                                        |
|--------------|:-------:|--------------------------------------------------------------------|
| $STD         | 0     | Default value <br> The behavior is similar to $FIXEDWIDTH.             |
| $FIXEDWIDTH  | 1     | Fixed width <br> Fit to the <a href="/package/extension3/tabframe/properties/tabwidth">TabWidth</a> property.                          |
| $MULTILINE   | 2     | Multi-line display <br><small><span style="color:blue">Not supported in AI</span></small>                            |
| $RAGGEDRIGHT | 3     | Width adjustment <br>Match the number of characters in TabForm.<a href="/package/extension3/tabform/properties/title">Title</a>. |

If $ TABRIGHT or $ TABLEFT is specified in the <a href="/package/extension3/tabframe/properties/tabposition">TabPosition</a> property (horizontal tab), the specification of this property is invalid. The operation is the same as when $ MULTILINE is specified.


If $ MULTILINE is set, the display will be undefined when the width of one tab exceeds TabFrame.Width. Do not enter a long string in TabForm.<a href="/package/extension3/tabform/properties/title">Title</a> that exceeds the width.