---
layout: default

parent: 2. Standard Package
has_children: true

title: CheckBox Class
nav_order: 2
permalink: /package/standard/checkbox

---
{% assign img1 = "/img/Biz Browser V/CheckBox_1.png" %}
{% assign img2 = "/img/Biz Browser V/CheckBox_2.png" %}

# {{ page.title }}

<a href="/img/Package/Standard-Checkbox.PNG" target="blank"><img src="/img/Package/Standard-Checkbox.PNG" alt="Standard-Checkbox"></a>


A class that displays a checkbox that allows you to select any number from multiple choices.

The CheckBox class works in tandem with the [CheckItem](/package/standard/checkitem) class.
To set the data to be displayed as a choice, you need to place the CheckItem class or its derived class objects in the structure defined under the CheckBox object.

<b>Object structure</b>

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<b>Screen display example</b>

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

<b>Printer output by Doc class</b>

On the left side of the character string, ■ indicating the selected status or □ indicating the non-selected status is printed.

<b>Default properties and ValueType</b>

The default property is [Value](/package/standard/checkbox/properties/value). The ValueType specification is invalid.

<b>Restrictions when visual style is enabled</b>

◆ The FgColor property is disabled and follows the OS theme.

<b>Precautions when scaling</b>

Nothing in particular