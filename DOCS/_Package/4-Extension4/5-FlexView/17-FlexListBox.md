---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexListBox Class
nav_order: 17
permalink: /package/extension4/flexview/flexlistbox

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/Ext4-FlexView-FlexListBox.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexListBox.PNG" alt="login image"></a>

The FlexListBox class defines how the cells in FlexView are displayed, and the corresponding cells are displayed like a pull-down list.

Place the FlexListBox object under the FlexRecord, FlexColumnSet, or FlexRowSet objects.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlistbox.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Layout Constraint**<br>
The FlexListBox object cannot be placed to the left (previous in definition order) of the objects in the FlexHeader class and its derived classes.

When located as a child of FlexRowSet and FlexColumnSet, it cannot co-exist with objects in the FlexHeader class and its derived classes.

**Default properties and ValueType**<br> 
The default property is <a href="/package/extension4/flexview/flexlistbox/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">Value Type can be specified since Ver.5.0.3</span></small>