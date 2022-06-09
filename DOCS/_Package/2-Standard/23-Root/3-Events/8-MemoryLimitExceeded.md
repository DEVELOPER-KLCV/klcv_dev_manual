---
layout: default

grand_parent: Root Class
parent: Events
has_children: false
title: Root.MemoryLimitExceeded Event
nav_order: 8
permalink: /package/standard/root/events/memorylimitexceeded
---
# {{ page.title }}
<br>

This event occurs only once when the memory usage exceeds the threshold specified by the SetMemoryLimitThreshold method.See the SetMemoryLimitThreshold method for details.<br><br>

The following child objects are attached to the Event object.<br>

| Type   | Name       | Description                                                                             |
|--------|------------|-----------------------------------------------------------------------------------------|
| Number | UsedMemory | The memory usage at the time when the threshold is exceeded is stored. The unit is MB . |


<br><small><span style="color:red">Can only be used in AI</span></small>
<br><small><span style="color:red">Added since AI Ver.1.0.1</span></small>
