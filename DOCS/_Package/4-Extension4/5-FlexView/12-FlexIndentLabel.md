---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexIndentLabel Class
nav_order: 12
permalink: /package/extension4/flexview/flexindentlabel

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<a href="/img/Package/Ext4-FlexView-FlexIndentLabel.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexIndentLabel.PNG" alt="login image"></a>

The FlexIndentLabel class is a class that defines how FlexView cells are displayed.

FlexIndentLabel is a class derived from FlexLabel and can display strings and icons in the same way as FlexLabel. In addition, indented display can be performed by specifying the Key property and ParentKey property. This display is similar to FlexTreeHeader, but FlexIndentLabel is a hierarchical display in one column, and the depth of the hierarchy changes dynamically depending on the data set in the Key and ParentKey properties. Also, the part that can be collapsed is only the beginning of the indent, but the contents of the following columns are also displayed in the collapsed row.
 
Place the FlexIndentLabel object below the FlexRecord object.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexilabel.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Layout Constraint**<br>
FlexIndentLabel objects cannot be placed to the left (previous in definition order) of objects in FlexHeader and its derived classes.

FlexIndentLabel cannot be used in more than one column. 

It can be placed as a child of FlexColumnSet, but the indented connecting lines are not connected. 

**Default properties and ValueType**<br> 
The default property is <a href="/package/extension4/flexview/flexindentlabel/properties/value">Value</a>. ValueType can be String Number, Fixed, Date and UString.<br><small><span style="color:green">UString have been added since Ver.4.2.0</span></small>