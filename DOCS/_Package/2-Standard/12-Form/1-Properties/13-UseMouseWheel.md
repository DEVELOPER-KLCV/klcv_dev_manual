---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Form.UseMouseWheel property
nav_order: 13
permalink: /package/standard/form/properties/usemousewheel
---
# {{ page.title }}


Specifies the condition for the MouseWheel event to notify the rotation of the mouse wheel.

Specify the occurrence condition by combining the following values.

| Constant     | Value | Description                                                                  |
|--------------|:-----:|------------------------------------------------------------------------------|
| $ STD        |   0   | The MouseWheel event does not occur.                                         |
| $ LEFTCLICK  |   1   | The MouseWheel event is fired while holding down the left mouse button.      |
| $ RIGHTCLICK |   2   | The MouseWheel event is fired while holding down the left mouse button.      |
| $ SHIFTKEY   |   4   | The MouseWheel event is fired while holding down the Shift key on keyboard . |
| $ CTRLKEY    |   8   | The MouseWheel event is fired while holding down the Ctrl key on keyboard .  |
| $ ANYTIME    |   31  | The MouseWheel event is fired in all states .                                |

Specify as below to raise the event only when the Ctrl key or the left mouse button is pressed.

```
UseMouseMove = $ LEFTCLICK + $ CTRLKEY;
```

If $ ANYTIME is specified, the event will be fired regardless of the state of the button or key. If you want to suppress the event only for a specific condition, subtract the condition you want to suppress from $ ANYTIME. For example, specify as below to suppress the event only when the right mouse click is pressed.

```
UseMouseMove = $ANYTIME - $RIGHTCLICK;
```

MouseWheel events generate a large number of events in conjunction with the rotation of the mouse wheel. If the event handler takes a long time to process, the responsiveness of the computer may be significantly reduced, so be careful to minimize the occurrence of events when and under the necessary conditions.

<br><small><span style="color:red">Added since Ver.5.0.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>