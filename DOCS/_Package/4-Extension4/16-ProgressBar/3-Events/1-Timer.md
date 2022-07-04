---
layout: default

grand_parent: ProgressBar Class
parent: Events
has_children: false
title: ProgressBar.Timer Event
nav_order: 1
permalink: /package/extension4/progressbar/events/timer
---
# {{ page.title }}

Occurs after each step of the progress bar.

This event only occurs when the <a href="/package/extension4/progressbar/methods/autostep">AutoStep</a> method specifies that the Timer event should occur.

 
The following child objects are attached to the Event object.

|  Type  |    Name    |       Description       |
|:------:|:----------:|:-----------------------:|
| Number | **_step_** | Current number of steps |

If you call the <a href="/package/extension4/progressbar/methods/stepit">StepIt</a> method in the OnTimer event handler by executing the AutoStep method, the progress bar will stop auto-progressing and the Timer event will not occur.