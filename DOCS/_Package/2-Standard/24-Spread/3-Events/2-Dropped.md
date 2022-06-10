---
layout: default

grand_parent: Spread Class
parent: Events
has_children: false
title: Dropped Event
nav_order: 2
permalink: /package/standard/spread/events/dropped
---
# {{ page.title }}
<br>

It is an event that occurs when it is dropped by drag and drop operation.<br><br>

A <a href="/package/extension4/droppedevent">DroppedEvent</a>
 object is passed as an argument to the OnDropped event handler.<br><br>

It may occur multiple times depending on the dropped content. For example, if multiple files are dropped from Explorer, the event will occur several times for that file.<br><br>

Events also occur when text data and files are dropped at the same time.

Example
```
Function OnDropped(e) {
    switch (e.Type) {
    case $STRING:
        print(e.Data, "\n");
        break;
    case $FILE:
        print(e.Data.PathName, "\n");
        break;
    }
}
```

