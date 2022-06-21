---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexGroupHeader Class
nav_order: 8
permalink: /package/extension4/flexview/flexgroupheader

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-FlexView-FlexGroupHeader.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexGroupHeader.PNG" alt="login image"></a>

The FlexGroupHeader class is a class that defines how to display the row headers of FlexView.

Corresponding header cells can display cell values and row numbers, similar to FlexHeader. Also, the horizontal scrolling is fixed and is always displayed on the left side, and the cursor cannot be placed.

The cells corresponding to FlexGroupHeader are displayed by key break of the cell value or grouped by the specified number of rows.

Place the FlexGroupHeader object under the FlexRecord or FlexColumnSet object.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexgheader.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Layout Constraint**<br>
FlexGroupHeader objects cannot be placed to the right (after in definition order) of objects of classes derived from FlexHeader and non-FlexHeader.

When positioned as a child of FlexColumnSet, it cannot live with objects of classes derived from anything other than FlexHeader.


**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/flexview/flexgroupheader/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">UString have been added since Ver.4.2.0</span></small>