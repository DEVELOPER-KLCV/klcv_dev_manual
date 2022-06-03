---
layout: default

parent: 2. Standard Package
has_children: true

title: Root Class
nav_order: 23
permalink: /package/standard/root

---


# {{ page.title }}
<br>

<a href="/img/Package/Standard-Root.PNG" target="_blank">
<img src="/img/Package/Standard-Root.PNG" alt="login image"></a>

The Root class is a class corresponding to the window of Biz / Browser itself, and has a function to determine the operation of Biz / Browser.

The Root object is at the top of all objects and is the starting point for the object tree.

Only one Root object is created in the application and can be accessed from anywhere by "//" on the CRS script.

For example, the value in the window title bar can be obtained with //.Title. 

The Root object has a special child object called the <a href="/package/standard/root/sysobject">SYSObject</a> that allows you to get system-specific information.

There is also a special function called OnException that handles global exceptions.

**Default properties and ValueType**

The default property is <a href="/package/standard/pulldownlist/properties/value">Value</a> . The ValueType specification is invalid.