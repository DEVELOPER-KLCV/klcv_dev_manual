---
layout: default

grand_parent: StyleEdit Class
parent: Events
has_children: false
title: StyleEdit.HotspotDoubleClicked Event
nav_order: 3
permalink: /package/extension4/styleedit/events/hotspotdoubleclicked
---
# {{ page.title }}

StyleEdit.HOTSPOT This event occurs when you double-click the left mouse button on a styled character.

The HotspotDoubleClicked event has the following structure:

```
Event {
    Number Style;
    Number Position;
    String Word;
}
```

Style stores the style number of the clicked part, Position stores the clicked character position, and Word stores the character string of the clicked part.