---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Form.UseMouseMove property
nav_order: 12
permalink: /package/standard/form/properties/usemousemove
---
# {{ page.title }}

<br>

Specifies the condition for the <a href="/package/standard/form/events/mousemove">MouseMove</a> event to notify the movement of the mouse pointer.

Specify the occurrence condition by combining the following values.

| Constant     | Value | Description                                                                 |
|--------------|:-----:|-----------------------------------------------------------------------------|
| $ STD        |   0   | The MouseMove event does not occur.                                         |
| $ LEFTCLICK  |   1   | The MouseMove event is fired while holding down the left mouse button.      |
| $ RIGHTCLICK |   2   | The MouseMove event is fired while holding down the left mouse button.      |
| $ SHIFTKEY   |   4   | The MouseMove event is fired while holding down the Shift key on keyboard . |
| $ CTRLKEY    |   8   | The MouseMove event is fired while holding down the Ctrl key on keyboard .  |
| $ ANYTIME    |   31  | The MouseMove event is fired in all states .                                |

Specify as below to raise the event only when the Ctrl key or the left mouse button is pressed.

```
UseMouseMove = $ LEFTCLICK + $ CTRLKEY;
```

If $ ANYTIME is specified, the event will be fired regardless of the state of the button or key. If you want to suppress the event only for a specific condition, subtract the condition you want to suppress from $ ANYTIME. For example, specify as below to suppress the event only when the right mouse click is pressed.

```
UseMouseMove = $ANYTIME - $RIGHTCLICK;
```

The MouseMove event causes a large number of events as the mouse moves. If the event handler takes a long time to process, the responsiveness of the computer may be significantly reduced, so be careful to minimize the occurrence of events when and under the necessary conditions.


<br><small><span style="color:blue">Not supported in AI</span></small>