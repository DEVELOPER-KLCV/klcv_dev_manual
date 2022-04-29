---
layout: default

grand_parent: STree Class
parent: Events
has_children: false
title: STree.Dropped Event
nav_order: 3
permalink: /package/extension5/stree/events/dropped
---
# {{ page.title }}

It is an event that occurs when it is dropped by drag and drop operation.

The event is in the form of an item accessor added to the [DroppedEvent]() class.

The following child objects are attached to the DroppedEvent object.

|Type       | Name          | Explanation         |
|-----------|---------------|---------------------|
| STreeItem | <b>item</b>   |STreeItem object that is an accessor to the dropped item |
 
 If dropped on an item in the tree, <b>item</b> will contain the accessor for the dropped item.

If dropped on something other than an <b>item</b> in the tree, the item will contain an invalid accessor ([Id](/package/extension5/streeitem/properties/id) property 0).