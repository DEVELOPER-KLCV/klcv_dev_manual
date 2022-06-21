---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexHeader Class
nav_order: 10
permalink: /package/extension4/flexview/flexheader

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/Ext4-FlexView-FlexHeader.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexHeader.PNG" alt="login image"></a>

The FlexHeader class is a class that defines how to display the row headers of FlexView.

The corresponding header cell can display the cell value or the row number. Also, the horizontal scrolling is fixed and is always displayed on the left side, and the cursor cannot be placed.

Place the FlexHeader object under the FlexRecord, FlexColumnSet, or FlexRowSet objects.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexheader.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Layout Constraint**<br>
FlexHeader objects cannot be placed to the right (after in definition order) of objects in classes derived from anything other than FlexHeader.

When positioned as a child of FlexRowSet and FlexColumnSet, it cannot co-exist with objects of classes derived from anything other than FlexHeader.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/flexview/flexheader/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">UString have been added since Ver.4.2.0</span></small>