---
layout: default

grand_parent: Form Class
parent: Events
has_children: false
title: Form.MouseWheel Event
nav_order: 8
permalink: /package/standard/form/events/mousewheel
---
# {{ page.title }}


<br>

Occurs when operating a mouse wheel that meets the conditions specified in the UseMouseWheel property. By processing with the OnMouseWheel event handler, it is possible to detect the operation of the mouse wheel.

If there is an object on the mouse pointer, that object takes precedence if it processes the mouse wheel.


The following child objects are attached to the Event object.

|  Type  |       Name      | Description                                                                                                                   |
|:------:|:---------------:|-------------------------------------------------------------------------------------------------------------------------------|
| Number |   **ShiftKey**  | 1 if the Shift key is pressed, 0 otherwise                                                                                    |
| Number |  **CtrlKeyKey** | 1 if the Ctrl key is pressed, 0 otherwise                                                                                     |
| Number |  **LeftButton** | 1 if the left mouse button is pressed, 0 otherwise                                                                            |
| Number | **RightButton** | 1 if the right mouse button is pressed, 0 otherwise                                                                           |
| Number |     **xPos**    | X coordinate of mouse pointer                                                                                                 |
| Number |     **yPos**    | Y coordinate of mouse pointer                                                                                                 |
| Number |    **delta**    | Mouse wheel rotation Upward rotation is indicated by a positive value and downward rotation is indicated by a negative value. |



<br><small><span style="color:red">Added since Ver.5.0.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>






























