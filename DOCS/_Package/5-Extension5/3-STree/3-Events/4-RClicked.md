---
layout: default

grand_parent: STree Class
parent: Events
has_children: false
title: STree.RClicked Event
nav_order: 4
permalink: /package/extension5/stree/events/rclicked
---
# {{ page.title }}

Occurs when the right mouse button is pressed.

The following child objects are attached to the Event object.

|Type       | Name               | Explanation         |
|-----------|--------------------|---------------------|
| STreeItem | <b>item</b>        | [STreeItem](/package/extension5/streeitem) object that is an accessor to the right-clicked item |
| Number    | <b>ShiftKey</b>    | 1 if the Shift key is pressed, 0 otherwise |
| Number    | <b>CtrlKey</b>     | 1 if the Ctrl key is pressed, 0 otherwise |
| Number    | <b>AltKey</b>      | 1 if the Alt key is pressed, 0 otherwise |
| Number    | <b>xPos</b>   | X coordinate of mouse pointer |
| Number  | <b>yPos</b> | Y coordinate of mouse pointer |

If an item in the tree is right-clicked, <b>item</b> contains the accessors for the right-clicked item.

If a non-item in the tree is right-clicked, the <b>item</b> will contain an invalid accessor ([Id](/package/extension5/streeitem/properties/id) property 0).