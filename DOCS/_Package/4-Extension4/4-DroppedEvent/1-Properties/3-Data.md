---
layout: default

grand_parent: DroppedEvent Class
parent: Properties
has_children: false
title: DroppedEvent.Data Property
nav_order: 3
permalink: /package/extension4/droppedevent/properties/data
---
# {{ page.title }}

The dropped data. The object that matches the data format of the <a href="/package/extension4/droppedevent/properties/type">Type</a> property is set.

| Type property | Object stored in Data property |
|---------------|--------------------------------|
| $ STRING      | String object                  |
| $ FILE        | File object                    |
| $ OBJECT      | Object set by source           |

Example of use
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
