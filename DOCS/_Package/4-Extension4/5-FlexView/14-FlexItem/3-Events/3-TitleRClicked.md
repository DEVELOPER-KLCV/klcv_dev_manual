---
layout: default

grand_parent: FlexItem Class
parent: Events
has_children: false
title: FlexItem.TitleRClicked Event
nav_order: 3
permalink: /package/extension4/flexview/flexitem/events/titlerclicked
---
# {{ page.title }}

This event occurs when click the right mouse on the title.

The TitleRClicked event has the following structure:

```
Event {
    Number ShiftKey;
    Number CtrlKey;
    Number AltKey;
}
```

ShiftKey, CtrlKey, and AltKey indicate the key press state when an event occurs, respectively.