---
layout: default

grand_parent: 2. Standard Package
parent: Root Class

title: Root.OnException Method
nav_order: 5
permalink: /package/standard/root/onexception

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}
<br>

This is a special function that is called directly from the CRS execution engine.

This function is called when a try ... catch raises an unhandled exception.

 

If true is returned as the return value, the CRS engine will continue processing without stopping.

If a value other than true is returned, the CRS execution engine will stop.

 

For details, refer to the "<a href="/bizBrowserV/3/3-15/">Exception Handling</a>"-"Global Exception Handler" section.


<br><small><span style="color:red">Added since Ver.4.0.0, Mobile Ver.3.0.0</span></small>
