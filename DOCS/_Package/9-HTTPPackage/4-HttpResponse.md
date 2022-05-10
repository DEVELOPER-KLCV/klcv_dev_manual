---
layout: default

parent: 9. HTTP Package
has_children: true

title: HttpResponse Class
nav_order: 4
permalink: /package/httppackage/httpresponse

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

A class that holds HTTP responses.

Get the HttpResponse object as the return value of the [HttpSession.Get]() or [HttpSession.Post]() method.

Among the errors that occurred in the communication process, the error that occurred in the HTTP layer is identified by the [Status]() property of the HttpResponse object. Note that even if you receive an HttpResponse object as a result of the HttpSession.Get, Post method, the communication may not complete successfully.

Also, even if the Status property indicates an error such as $HTTP_NOT_FOUND, the [Body]() property may contain meaningless values ​​such as HTML containing the error message returned by the WEB server.

**Default properties and ValueType**
 
The default property is [Body](). The ValueType specification is invalid.