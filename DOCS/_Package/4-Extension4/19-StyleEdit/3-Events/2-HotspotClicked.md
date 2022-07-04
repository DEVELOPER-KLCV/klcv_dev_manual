---
layout: default

grand_parent: StyleEdit Class
parent: Events
has_children: false
title: StyleEdit.HotspotClicked Event
nav_order: 2
permalink: /package/extension4/styleedit/events/hotspotclicked
---
# {{ page.title }}

StyleEdit.HOTSPOT This event occurs when you left-click the mouse on a styled character.

The HotspotClicked event has the following structure:

```
Event {
    Number Style;
    Number Position;
    String Word;
}
```

Style stores the style number of the clicked part, Position stores the clicked character position, and Word stores the character string of the clicked part.