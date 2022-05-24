---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Form.UseGesture property
nav_order: 11
permalink: /package/standard/form/properties/usegesture
---
# {{ page.title }}


<br>
Specifies the type of gesture to capture in the <a href="/package/standard/form/events/gesture">Gesture</a> event.

Specify the occurrence condition by combining the following values.

| Constant         |    Value   | Description                                                                                                                                                                                                                                                                                                            |
|------------------|:----------:|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| $ STD            |      0     | The Gesture event does not occur.                                                                                                                                                                                                                                                                                      |
| $ FLICK          |      1     | Captures a flick operation and raises a Gesture event. $ NOPARENTSCROLL must be specified at the same time.                                                                                                                                                                                                            |
| $ SWIPE          |      2     | Captures a swipe operation and raises a Gesture event. $ NOPARENTSCROLL must be specified at the same time.                                                                                                                                                                                                            |
| $ PINCH          |      4     | Captures a pinch operation and raises a Gesture event.                                                                                                                                                                                                                                                                 |
| $ NOPARENTSCROLL | 0x00010000 | If this value is specified, it captures panning operations (scrolling, flicking, swiping, etc.) on its own area. If not specified, flick and swipe operations are forwarded to the parent form. Also, scrolling operations are captured by themselves if they scroll, otherwise they are forwarded to the parent form. |

Specify as below to capture flick and swipe operations.

```
UseGesture = $ FLICK + $ SWIPE + $ NOPARENTSCROLL;
```

Specify as below to capture a pinch operation.

```
UseGesture = $ PINCH;
```

Gesture events by swipe operation and pinch operation generate a large number of events in conjunction with the operation. If it takes a long time to process the event handler, the responsiveness of the terminal may be greatly reduced, so please be careful to minimize the occurrence of events when and under the necessary conditions.

<br><small><span style="color:red">Added since Ver.5.0.4</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>