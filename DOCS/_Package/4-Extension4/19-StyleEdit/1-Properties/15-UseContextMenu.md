---
layout: default

grand_parent: StyleEdit Class
parent: Properties
has_children: false
title: StyleEdit.UseContextMenu Property
nav_order: 15
permalink: /package/extension4/styleedit/properties/usecontextmenu
---
# {{ page.title }}

Specifies whether to use the context menu that appears when you right-click the mouse.

If $TRUE is specified, the standard context menu is displayed, but the ContextMenu event is not fired.

If $FALSE is specified, the ContextMenu event is fired, but the context menu is not displayed.

The behavior can be customized when right-clicking by specifying false for UseContextMenu and defining an OnContextMenu event handler.

```
StyleEdit obj {
    :
    UseContextMenu = $FALSE;
    :
    Function OnContextMenu(e) {
        var sel = PopupMenu("menu1", "menu2", "menu3");
        MessageBox("menu" + str(sel) + " selected");
    }
}
```

<small><span style="color:red">Added since Ver.4.1.3</span></small>