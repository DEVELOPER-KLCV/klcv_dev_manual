---
layout: default

parent: 9. HTTP Package
has_children: true

title: HttpSession Class
nav_order: 5
permalink: /package/httppackage/httpsession

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that holds HTTP session information. Manages the connection with the WEB server.

This class supports http, https, and file protocols, and is implicitly generated and used at login and in the Form.Get method. It is also possible to use the HttpSession class and [HttpRequest](/package/httppackage/httprequest) class directly for more advanced communication.

Biz / Browser maintains multiple objects of HttpSession class for each connection destination. Communication to the same destination reuses the already maintained HttpSession object.

The HttpSession object can be obtained with the static method [GetSession](/package/httppackage/httpsession/methods/getsession) or [FindSession](/package/httppackage/httpsession/methods/findsession) and the global function [getHttpSession](/method/system/gethttpsession) or [findHttpSession](/method/system/findhttpsession).

**Default properties and ValueType**

The default property is [Server](/package/httppackage/httpsession/properties/server). The ValueType specification is invalid.