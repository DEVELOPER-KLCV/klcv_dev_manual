---
layout: default

grand_parent: FlexItem Class
parent: Events
has_children: false
title: FlexItem.TitleDClicked Event
nav_order: 1
permalink: /package/extension4/flexview/flexitem/events/titledclicked
---
# {{ page.title }}

This event occurs when double-clicking the left mouse on the title.

The TitleDClicked event has the following structure:

```
Event {
    Number ShiftKey;
    Number CtrlKey;
    Number AltKey;
}
```

ShiftKey, CtrlKey, and AltKey indicate the key press state when an event occurs, respectively.