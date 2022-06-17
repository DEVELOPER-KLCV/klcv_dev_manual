---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexButton Class
nav_order: 1
permalink: /package/extension4/flexview/flexbutton

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-FlexView-FlexButton.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexButton.PNG" alt="login image"></a>

The FlexButton class is a class that defines how cells in FlexView are displayed, and the corresponding cells are displayed like buttons.

Place the FlexButton object under a FlexRecord object, FlexColumnSet object, or FlexRowSet object.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexbutton.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Constraint Layout** 

FlexButton objects cannot be placed to the left (previous in definition order) of objects in the FlexHeader class and its derived classes.

When located as a child of FlexRowSet and FlexColumnSet, it cannot co-exist with objects in the FlexHeader class and its derived classes.

**Default properties and ValueType**<br>

The default property is <a href="/package/extension4/flexview/flexbutton/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">Value Type can be specified since Ver.4.2.0</span></small> 








