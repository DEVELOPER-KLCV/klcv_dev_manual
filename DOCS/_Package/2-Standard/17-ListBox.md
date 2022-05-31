---
layout: default

parent: 2. Standard Package
has_children: true

title: ListBox Class
nav_order: 17
permalink: /package/standard/listbox

---


# {{ page.title }}

<br>

<a href="/img/Package/Standard-ListBox.PNG" target="_blank">
<img src="/img/Package/Standard-ListBox.PNG" alt="login image"></a>

<br>

This class displays a list box.

The ListBox class works in tandem with the ListItem class.

To set the data to be displayed as choices, you need to place an object of ListItem or its derived class in the structure defined under the ListBox object.

<br>

**Object Structure**

<a href="/img/Package/Standard-ListBox-Object.PNG" target="_blank">
<img src="/img/Package/Standard-ListBox-Object.PNG" alt="login image"></a>

<br>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std9.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br>

**Printer output by Doc class**

The selected character string is highlighted, and the non-selected character string is displayed normally.

 <br>


**Default properties and ValueType**
 

The default property is <a href="/package/standard/form/properties/value">Value</a>. The ValueType specification is invalid.


 <br>
 
**Restrictions when visual style is enabled**

Nothing in particular.

<br>

**Precautions when scaling** 

Nothing in particular.