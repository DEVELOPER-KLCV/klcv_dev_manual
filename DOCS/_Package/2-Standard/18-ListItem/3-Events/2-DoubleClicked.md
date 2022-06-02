---
layout: default

grand_parent: ListItem Class
parent: Events
has_children: false
title: ListItem.DoubleClicked Property
nav_order: 2
permalink: /package/standard/listitem/events/doubleclicked
---
# {{ page.title }}
<br>
Occurs when the left mouse button is double-clicked.

 

The following child objects are attached to the Event object.

|  Type  | Name           | Description                                |
|:------:|----------------|--------------------------------------------|
| Number |  **ShiftKey**  | 1 if the Shift key is clicked, 0 otherwise |
| Number | **CtrlKey** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |   **AltKey**   | 1 if the Alt key is clicked, 0 otherwise   |
| Number |    **xPos**    | X coordinate of mouse pointer              |
| Number |    **yPos**    | Y coordinate of mouse pointer              |

***Note***<br>
In the handler of the event that occurred in the ListItem class, do not use the <a href="/package/standard/listbox/properties/value">Value</a> property of the parent object <a href="/package/standard/listbox">ListBox</a> class to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the <a href="/package/system/event/properties/from">From</a> property (ListItem object) of the <a href="/package/system/event">Event</a> object passed as an argument of the event handler. For the selected state of the item, refer to the <a href="/package/standard/listitem/properties/selected">Selected</a> property from the From property. 
