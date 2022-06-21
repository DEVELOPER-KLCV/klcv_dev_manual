---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexLabel Class
nav_order: 15
permalink: /package/extension4/flexview/flexlabel

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/Ext4-FlexView-FlexLabel.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexLabel.PNG" alt="login image"></a>

The FlexLabel class is a class that defines how cells in FlexView are displayed, and the corresponding cells are displayed like labels.

Place the FlexLabel object under the FlexRecord, FlexColumnSet, or FlexRowSet objects.

If specify the verticalAlign property, the characters in the FlexLabel cannot be wrapped. If do not specify the verticalAlign property, the characters in the FlexLabel are wrapped.

If the character does not fit within the right edge of the display range, it will be displayed on the next row with a line break. The line wrap is considered for the line break position, and if no word break is found in the alphabet, the line break is not performed.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexlabel.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Layout Constraint**<br>
FlexLabel objects cannot be placed to the left (previous in definition order) of objects in the FlexHeader class and its derived classes.

When located as a child of FlexRowSet and FlexColumnSet, it cannot co-exist with objects in the FlexHeader class and its derived classes.

**Default properties and ValueType**<br> 
The default property is <a href="/package/extension4/flexview/flexlabel/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">UString have been added since Ver.4.2.0</span></small>