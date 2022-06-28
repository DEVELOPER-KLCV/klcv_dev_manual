---
layout: default

grand_parent: ListView Class
parent: Events
has_children: false
title: Dropped Event
nav_order: 3
permalink: /package/extension4/listview/events/dropped
---
# {{ page.title }}

It is an event that occurs when it is dropped by drag and drop operation.

A <a href="/package/extension4/droppedevent">DroppedEvent</a> object is passed as an argument to the OnDropped event handler.

It may occur multiple times depending on the dropped content. For example, if multiple files are dropped from Explorer, the event will occur several times for that file.
Events will also occur if text data and files are dropped at the same time.

Usage Example

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

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>