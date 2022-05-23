---
layout: default

parent: 2. Standard Package
has_children: true

title: Form Class
nav_order: 12
permalink: /package/standard/form

---

# {{ page.title }}

<a href="/img/Package/Standard-Form.PNG" target="_blank">
<img src="/img/Package/Standard-Form.PNG" alt="login image"></a>

A class that displays a form.

 

Place and manage another object at the bottom of the form. Subordinate objects are never displayed beyond the area of ​​the parent Form object to which they belong , and are clipped by the size of the parent Form object.

**Screen display example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std19.files/image001.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output using Doc class**

Form objects represent areas on paper. Unlike when displayed on the screen, printing is performed without clipping even if the child object is located at a position beyond the display range of the Form object.

**Default properties and ValueType**
 

The default property is <a href="/package/standard/form/properties/value">Value</a>. ValueType can be String , Number , Fixed , Date , UString.
<br><small><span style="color:green">UString has been added from Ver.4.2.0</span></small>

**Restrictions when visual style is enabled**

Nothing in particular

**Precautions when scaling** <br>
◆ It is scaled by the scaling value of the upper Form object.

◆ The lower object is scaled by multiplying the scaling value of the upper Form object by its own scaling value.

**Precautions for gesture operation** <small><span style="color:red">Added since Ver.5.0.4</span></small>

In Biz / Browser V 5.0.4.0 or later, the <a href="/package/standard/form/properties/usegesture">UseGesture</a> property and <a href="/package/standard/form/events/gesture">Gesture</a> event can be used to get the gesture by touch operation as an event.

For details, please refer to <a href="/bizBrowserV/2/2-8/">Gesture operation</a>.