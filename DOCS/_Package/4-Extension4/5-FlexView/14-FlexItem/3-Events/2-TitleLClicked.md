---
layout: default

grand_parent: FlexItem Class
parent: Events
has_children: false
title: FlexItem.TitleLClicked Event
nav_order: 2
permalink: /package/extension4/flexview/flexitem/events/titlelclicked
---
# {{ page.title }}

This event occurs when click the left mouse on the title.

The TitleLClicked event has the following structure:

```
Event {
    Number ShiftKey;
    Number CtrlKey;
    Number AltKey;
}
```

ShiftKey, CtrlKey, and AltKey indicate the key press state when an event occurs, respectively.