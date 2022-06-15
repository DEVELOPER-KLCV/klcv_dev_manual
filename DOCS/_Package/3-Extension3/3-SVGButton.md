---
layout: default

parent: 3. Extension3 Package
has_children: true

title: SVGButton Class
nav_order: 3
permalink: /package/extension3/svgbutton

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext3-SVGButton.PNG" target="_blank">
<img src="/img/Package/Ext3-SVGButton.PNG" alt="login image"></a>

A class that displays an SVG button that can display an SVG image on the surface.


**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext1.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
 The SVG of the <a href="/package/extension3/svgbutton/properties/image">Image</a> property is printed.

**Default properties and ValueType**<br>
 The default property is <a href="/package/extension3/svgbutton/properties/value">Value</a> . ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small><br><br>
 
**Restrictions when visual style is enabled**<br>
◆ Invalid visual style.


 **Precautions when scaling**<br>
◆ The SVG displayed in conjunction with the scaling of the SVGButton itself will also be scaled.