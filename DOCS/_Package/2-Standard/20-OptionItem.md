---
layout: default

parent: 2. Standard Package
has_children: true

title: OptionItem Class
nav_order: 20
permalink: /package/standard/optionitem

---


# {{ page.title }}

<br>

<a href="/img/Package/Standard-OptionItem.PNG" target="_blank">
<img src="/img/Package/Standard-OptionItem.PNG" alt="login image"></a>

<a href="/package/standard/optionbutton">OptionButton</a> A class that defines the choices of the class. Be sure to use it by arranging it as a child object of the OptionButton class.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std6.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

<br>

**Printer Output by Doc class**

◎ indicating the selected status or ○ indicating the non-selected status is printed on the left side of the character string.

<br>

**Default properties and ValueType**

The default property is <a href="/package/standard/optionitem/properties/value">Value</a> . ValueType can be String , Number , Fixed , Date , UString.

<small><span style="color:green">UString has been added since Mobile Ver.4.2.0</span></small>

<br>

**Restrictions when visual style is enabled**

Nothing in particular

<br>

**Precautions when scaling**
 
◆ Select button is not scaled