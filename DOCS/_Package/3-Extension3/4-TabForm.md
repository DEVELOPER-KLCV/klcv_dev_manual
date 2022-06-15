---
layout: default

parent: 3. Extension3 Package
has_children: true

title: TabForm Class
nav_order: 4
permalink: /package/extension3/tabform

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>


<a href="/img/Package/Ext3-TabForm.PNG" target="_blank">
<img src="/img/Package/Ext3-TabForm.PNG" alt="login image"></a>

A class that defines each tab of the <a href="/package/extension3/tabframe">TabFrame</a> class. Be sure to use it as a child object of the TabFrame class.

The TabForm class inherits the functionality of the <a href="/package/standard/form">Form</a> class, so objects can be placed underneath. Subordinate objects are never displayed beyond the area of the TabForm object to which they belong, and are clipped by the size of the TabForm object.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext5.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Default properties and ValueType**<br>
 The default property is <a href="/package/extension3/form/properties/value">Value</a> . ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small><br>
 
**Restrictions when visual style is enabled**<br>
◆ Specifying TabFgColor and TabBgColor is invalid.

 **Precautions when scaling**<br>
◆ The size of TabForm is automatically determined by the size of TabFrame, but the size is further corrected to correct the scaling error that occurs in TabFrame. Specifically, when enlarged, the size will be larger than the theoretical value.