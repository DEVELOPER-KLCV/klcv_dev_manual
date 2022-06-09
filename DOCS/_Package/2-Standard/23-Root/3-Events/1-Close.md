---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.Close Event
nav_order: 1
permalink: /package/standard/root/events/close
---
# {{ page.title }}
<br>

Occurs when the close button in the upper right corner of the root window is pressed.

 

If this event is caught by the event handler, the operation to close the window will be cancelled. If you want to close the window, delete the Root object in the event handler.


Example
```
Function OnClose(e) {
    if (...) {
        //.Delete();
    }
}
```


