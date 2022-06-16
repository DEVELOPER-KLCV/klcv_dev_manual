---
layout: default

grand_parent: TabFrame Class
parent: Properties
has_children: false
title: TabFrame.TabPosition Property
nav_order: 8
permalink: /package/extension3/tabframe/properties/tabposition
---
# {{ page.title }}
<br>

Set the tab position.

| Constant   | Value | Description                |
|------------|:-----:|----------------------------|
| $STD       |   0   | Top                        |
| $TABRIGHT  |   1   | Right <br><small><span style="color:blue">Not supported in AI</span></small> |
| $TABBOTTOM |   2   | Bottom                     |
| $TABLEFT   |   3   | Left <br><small><span style="color:blue">Not supported in AI</span></small>  |

If $ TABRIGHT or $ TABLEFT is specified, the <a href="/package/extension3/tabframe/properties/arrangement">Arrangement</a> property specification is invalid, and the operation is the same as when $ MULTILINE (multi-line display) is specified.