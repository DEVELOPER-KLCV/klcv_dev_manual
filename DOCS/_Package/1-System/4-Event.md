---
layout: default

parent: 1. System Package
has_children: true

title: Event Class
nav_order: 4
permalink: /package/system/event

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/System-Event.PNG" target="_blank">
<img src="/img/Package/System-Event.PNG" alt="login image"></a>

A class that represents an event that occurs in a CRS program, such as a button click.

It is also used when the [PostEvent](/package/system/object/methods/postevent) method raises an event from a CRS script. 

<b>Default properties and ValueType</b>
 
The default property is [Reason](/package/system/event/properties/reason). The ValueType specification is invalid.