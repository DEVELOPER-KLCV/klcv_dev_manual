---
layout: default

parent: 2. Standard Package
has_children: true

title: Button Class
nav_order: 1
permalink: /package/standard/button

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}

A class that displays buttons. The surface displays the value of the [Title](/package/standard/button/properties/title) property.

<b>Screen display example</b>

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<b>Printer output by Doc class</b>

Only the label is printed.

<b>Default properties and ValueType</b>
 
The default property is [Value](/package/standard/button/properties/value). ValueType can be String, Number, Fixed, Date, UString.<br>
**<small>UString was added since Version 4.2.0</small>**

<b>Restrictions when visual style is enabled</b>

Nothing in particular

<b>Precautions when scaling</b>
 
Nothing in particular