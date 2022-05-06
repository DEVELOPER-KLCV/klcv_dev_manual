---
layout: default

grand_parent: STree Class
parent: Events
has_children: false
title: STree.SelectChanged Event
nav_order: 5
permalink: /package/extension5/stree/events/selectchanged
---
# {{ page.title }}

It is an event that occurs in the item selection operation of STree.

The following child objects are attached to the Event object.

| Type     | Name        | Explanation    |
|----------|-------------|----------------|
|STreeItem | <b>item</b> | [STreeItem](/package/extension5/streeitem) object that is an accessor to the selected item |

If an item in the tree is selected, <b>item</b> will contain the accessors for the selected item.
If no item is selected, <b>item</b> will contain an invalid accessor ([Id](/package/extension5/streeitem/properties/id) property 0).

You can also get the selected position with the [SelectedItem](/package/extension5/stree/properties/selecteditem) property, but see <b>item</b> to make sure you identify the item where the event occurred.
Since the event goes through the event queue, it may point to an <b>item</b> that is different from the item passed to the OnSelectChanged event handler and the SelectedItem property at that time.