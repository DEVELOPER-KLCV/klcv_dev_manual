---
layout: default

parent: 10. Runtime Package
has_children: true

title: Runtime Class
nav_order: 3
permalink: /package/runtimepackage/runtime

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

The Runtime class is a collection of functions that strongly depend on the environment of each PC, and is a class that serves as a contact point with the operating system of the PC.

By using the Runtime class, you can operate environment variables, start external programs, call the shell function of Explorer, and so on.

**Default properties and ValueType**

The default property is [Value](/package/runtimepackage/runtime/properties/value). You can specify String, Number, Fixed, and Date for ValueType.

<b><u>Mobile version original extension</u></b>

As a function unique to Biz / Browser Mobile, it implements a mechanism for loading external DLLs and calling functions.

With this mechanism, it is possible to control hardware specific to mobile terminals and acquire values ​​from Biz / Browser Mobile via an external DLL.

<a href="/img/Biz Browser V/RuntimeClass.PNG" target="_blank">

<img src="/img/Biz Browser V/RuntimeClass.PNG" alt="runtime image">


<b><u>Android version original extension</u></b>

As a function unique to Biz / Browser AI, we have implemented a location information acquisition mechanism using GPS and mobile networks.
With this mechanism, you can easily perform processing based on the user's position and cooperation with other map applications.