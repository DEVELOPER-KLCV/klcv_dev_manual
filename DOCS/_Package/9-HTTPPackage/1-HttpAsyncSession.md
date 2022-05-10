---
layout: default

parent: 9. HTTP Package
has_children: true

title: HttpAsyncSession Class
nav_order: 1
permalink: /package/httppackage/httpasyncsession

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---
A class that manages background asynchronous communication.
This class can generate and manage multiple communications by ID, and communications are performed simultaneously and asynchronously in a thread separate from the CRS execution engine. After the communication is completed, the reception result will be notified together with the ID as an event.

As with the [HttpSession](/package/httppackage/httpsession) class, simple communication using the [Get](/package/httppackage/httpasyncsession/methods/get) and [Post](/package/httppackage/httpasyncsession/methods/post) methods, as well as advanced communication using the [HttpRequest](/package/httppackage/httprequest) class is possible.

Instances of this class should always be retained during communication. When the instance disappears, all communicating sessions are forcibly disconnected.

**Default properties and ValueType**

The default property is [Sessions](/package/httppackage/httpasyncsession/properties/sessions). The ValueType specification is invalid.