---
layout: default

parent: 2. Standard Package
has_children: true

title: CheckItem Class
nav_order: 3
permalink: /package/standard/checkitem

---
{% assign img1 = "/img/Biz Browser V/CheckItem_1.png" %}

# {{ page.title }}

A class that defines the choices of the [CheckBox](/package/standard/checkbox) class. Be sure to array and use it as a child object of CheckBox class.

<b>Screen display example</b>

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<b>Printer output by Doc class</b>
 
A check mark indicating the selection status is printed on the left side of the character string.

<b>Default properties and ValueType</b>
 
The default property is [Value](/package/standard/checkitem/properties/value). ValueType can be String, Number, Fixed, Date, UString.<br>
**<small>UString added since Version 4.2.0</small>**

<b>Restrictions when visual style is enabled</b>

Nothing in particular

<b>Precautions when scaling</b>
 
◆ Select button is not scaled