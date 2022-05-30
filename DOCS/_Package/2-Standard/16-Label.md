---
layout: default

parent: 2. Standard Package
has_children: true

title: Label Class
nav_order: 16
permalink: /package/standard/label

---


# {{ page.title }}

<br>

<a href="/img/Package/Standard-Label.PNG" target="_blank">
<img src="/img/Package/Standard-Label.PNG" alt="login image"></a>

<br>

A class that displays character labels.

The value of the <a href="/package/standard/label/properties/value">Value</a> property is formatted according to the specification of the <a href="/base/format">Format</a> property and displayed on the screen.

If the character does not fit within the right edge of the display range, it will be displayed on the next line with a line break. Word wrap is taken into consideration for the line feed position, and if no word break is found in the alphabet, no line break is performed.

If the line does not fit within the bottom of the display range, it will be clipped and the following lines will not be displayed.


<br>


**Screen display example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


<br>

**Printer output by Doc class**

It will be printed in the same way as the screen.

If the BorderStyle property is set to $ DASH or $ DOT, it will be printed according to the style, but in other cases, the border will always be a solid line and the specification of the BorderStyle property will be ignored. Even if you specify the UString type as the data type, all characters are converted to multibyte when printing, so Unicode-specific characters are printed as "?".

<br>

**Default properties and ValueType**
 

The default property is <a href="/package/standard/form/properties/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.
<br><small><span style="color:green">Added since Ver.4.2.0</span></small>

<br>

**Restrictions when visual style is enabled**

◆ Visual style specification is invalid.

<br>

**Precautions when scaling** 

Nothing in particular.