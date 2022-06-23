---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexTreeHeader Class
nav_order: 24
permalink: /package/extension4/flexview/flextreeheader

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/Ext4-FlexView-FlexTreeHeader.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexTreeHeader.PNG" alt="login image"></a>

The FlexTreeHeader class is a class that defines how to display the row headers of FlexView. The corresponding header cells are displayed as a key break of the cell value or grouped by the specified number of rows, similar to FlexGroupHeader.

FlexTreeHeader can display groups in a tree format and collapse or unfold the groups by operating the screen.

Place the FlexTreeHeader object under the FlexRecord or FlexColumnSet object.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flextheader.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Layout Constraint**<br>
FlexTreeHeader objects cannot be placed to the right (after in definition order) of objects of classes derived from FlexHeader, FlexGroupHeader, and non-FlexHeader.

When positioned as a child of FlexColumnSet, it cannot live with objects of classes derived from anything other than FlexTreeHeader.


**Default properties and ValueType**<br> 
The default property is <a href="/package/extension4/flexview/flextreeheader/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">Value Type can be specified since Ver.4.2.0</span></small> 