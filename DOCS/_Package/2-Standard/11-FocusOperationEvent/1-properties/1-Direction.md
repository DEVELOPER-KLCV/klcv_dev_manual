---
layout: default

grand_parent: FocusOperationEvent Class
parent: Properties
has_children: false
title: FocusOperationEvent.Direction property
nav_order: 1
permalink: /package/standard/focusoperationevent/properties/direction
---
# {{ page.title }}


The following values ​​are stored to indicate in which direction the focus was moved.

 | Constant    | Value | Description     |
|:-------------:|:-----:|:-----------------:|
| $ NEXTFOCUS |   1   | Next object     |
| $ PREVFOCUS |   2   | Previous object |

By passing the value of the Direction property to the <a href="/package/standard/focusobject/methods/movefocus">MoveFocus</a> method of the <a href="/package/standard/focusobject">FocusObject</a> class, you can move the focus in the same way as the original focus movement.

Example

```
Function OnFocusOperation (e) {
    if (Value == "") {
        BgColor = $ RED;
        MessageBox (" Enter ");
        return;
    }
    BgColor = $ STD;
    MoveFocus (e.Direction);
}
 
 ```