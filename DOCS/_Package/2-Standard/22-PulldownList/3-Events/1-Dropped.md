---
layout: default

grand_parent: PulldownList Class
parent: Events
has_children: false
title: Dropped Property
nav_order: 1
permalink: /package/standard/pulldownlist/events/dropped
---
# {{ page.title }}
<br>

This event occurs when a drag and drop operation is used to drop the item.

 

A <a href="/package/extension4/droppedevent">DroppedEvent</a> object is passed as an argument to the OnDropped event handler.

 

It may occur multiple times depending on the dropped content. For example, if multiple files are dropped from Explorer, the event will occur several times for that file.

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

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>