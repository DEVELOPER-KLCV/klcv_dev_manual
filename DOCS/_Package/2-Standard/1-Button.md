---
layout: default

parent: 2. Standard Package
has_children: true

title: Button Class
nav_order: 1
permalink: /package/standard/button

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std2.files/image001.gif" %}

# {{ page.title }}

<a href="/img/cvnet/1-1-common/common-login.PNG" target="_blank">


<a href="/img/Package/Standard-Button.PNG" target="blank"><img src="/img/Package/Standard-Button.PNG" alt="Standard-Button"></a>



A class that displays buttons. The surface displays the value of the [Title](/package/standard/button/properties/title) property.

<b>Screen display example</b>

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


<b>Printer output by Doc class</b>

Only the label is printed.

<b>Default properties and ValueType</b>
 
The default property is [Value](/package/standard/button/properties/value). ValueType can be String, Number, Fixed, Date, UString.<br>
**<small>UString was added since Version 4.2.0</small>**

<b>Restrictions when visual style is enabled</b>

◆ Visual style specification is invalid

<b>Precautions when scaling</b>
 
Nothing in particular