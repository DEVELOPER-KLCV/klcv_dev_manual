---
layout: default

parent: 1. System Package
has_children: true

title: NetObject Class
nav_order: 8
permalink: /package/system/netobject

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The base class of a class in which a CRS file can be executed. It has a communication function with a WEB server and a function to compile and execute downloaded CRS files, and a class derived from the NetObject class can execute a new CRS program by using the [Get]() method or the like.

The NetObject class is a virtual class and cannot instantiate itself.

In the Mobile version, there is no NetObject class because there is no concept of class, but in the explanation of common properties and methods, it is explained as NetObject class for convenience.