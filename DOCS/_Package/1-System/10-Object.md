---
layout: default

parent: 1. System Package
has_children: true

title: Object Class
nav_order: 10
permalink: /package/system/object

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The base class for all classes. All the classes contained in Biz / Browser are derived from the Object class.

The Object class has the most basic functions of an object, such as managing the object tree and maintaining and opening the object.

The Object class is a virtual class and cannot instantiate itself.

In the Mobile version, the Object class does not exist because there is no concept of class, but in the explanation of common properties and methods, it is explained as Object class for convenience.