---
layout: default

grand_parent: 2. Standard Package
parent: Root Class

title: Events
nav_order: 3
permalink: /package/standard/root/events

---


# {{ page.title }}

The following events are defined in the Root class.

|Name       |  Description |
|----------	|--------------|
|[Close](/package/standard/root/events/close) | Occurs when closing the root window|
|[MenuSelected](/package/standard/root/events/menuselected) |Occurs when selecting the main menu<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add500.gif" alt="Image" width="50" height="12"></span></small><br><small><span style="color:blue">Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"></span></small> |
|[WindowStateChanged](/package/standard/root/events/windowstatechanged) |Occurs when the root window state changes<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add413.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12"></span></small><br><small><span style="color:green">The function has been expanded since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-change321.gif" alt="Image" width="86" height="12"></span></small> |

Only available for Mobile version

|Name       |  Description |
|----------	|--------------|
|[ExternalCall](/package/standard/root/events/externalcall) |Occurs when receiving a notification from an external program <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add320.gif" alt="Image" width="86" height="12"></span></small>|
|[PowerStateChanged](/package/standard/root/events/powerstatechanged) | Occurs when the device waking up from sleep (suspend)<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add400.gif" alt="Image" width="86" height="12"></span></small>|

Only available for Android version

|Name       |  Description |
|----------	|--------------|
|[MemoryLimitExceeded](/package/standard/root/events/memorylimitexceeded) | Occurs when the memory usage set by the MemoryLimitThreshold property is exceeded<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add101.gif" alt="Image" width="65" height="12"></span></small>|
|[ExternalMessage](/package/standard/root/events/externalmessage) | Obtained with ExternalObject.getMessageHandler<br>Occurs when a message is received by the message handler<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add102.gif" alt="Image" width="65" height="12"></span></small>|
|[ExternalIntent](/package/standard/root/events/externalintent) | Occurs when receiving an Intent from another app<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-add102.gif" alt="Image" width="65" height="12"></span></small>|