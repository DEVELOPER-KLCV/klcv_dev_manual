---
layout: default

grand_parent: TreeView Class
parent: Events
has_children: false
title: Dropped Event
nav_order: 2
permalink: /package/extension3/treeview/events/dropped
---
# {{ page.title }}
<br>

It is an event that occurs when it is dropped by drag and drop operation.

A <a href="/package/extension4/droppedevent/">DroppedEvent</a> object is passed as an argument to the OnDropped event handler.

It may occur multiple times depending on the dropped content. For example, if multiple files are dropped from Explorer, the event will occur several times for that file.

The event also occurs when the text data and the file are dropped at the same time.

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

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>