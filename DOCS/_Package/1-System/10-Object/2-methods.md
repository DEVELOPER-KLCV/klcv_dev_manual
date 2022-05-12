---
layout: default

grand_parent: 1. System Package
parent: Object Class

title: Methods
nav_order: 2
permalink: /package/system/object/methods

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following methods are defined in the Object class.

|  Name | Description |
|-------|-------------|
|[Append](/package/system/object/methods/append)|Connects the specified object to the object tree |
|[Clear](/package/system/object/methods/clear)|Initializes the object's default properties |
|[ClearChild](/package/system/object/methods/clearchild)|Initializes the default properties of all child objects |
|[Delete](/package/system/object/methods/delete)|Disconnect the object from the object tree |
|[DeleteChild](/package/system/object/methods/deletechild)|Disconnects all child objects from the object tree |
|[FindChild](/package/system/object/methods/findchild)|Finds a child object with the specified name<br><small>Added since Version 4.0.0<br> Not supported on mobile</small> |
|[FindObject](/package/system/object/methods/findobject)|Find an object from the object tree<br><small>Added since Version 4.1.3<br> Not supported on mobile</small> |
|[GetChildObjects](/package/system/object/methods/getchildobjects)|Gets all child objects<br><small>Added since Version 3.0.0</small> |
|[PostEvent](/package/system/object/methods/postevent)|Send an event to the object |

Methods only for array objects

|  Name | Description |
|-------|-------------|
|[Insert](/package/system/object/methods/insert)|Add an element to the array object |
|[Truncate](/package/system/object/methods/truncate)|Deletes all elements of the array object|