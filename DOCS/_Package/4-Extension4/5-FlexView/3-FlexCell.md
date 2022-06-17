---
layout: default

grand_parent: 4. Extension4 Package
parent: FlexView Class
has_children: true

title: FlexCell Class
nav_order: 3
permalink: /package/extension4/flexview/flexcell

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-FlexView-FlexCell.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView-FlexCell.PNG" alt="login image"></a>

The FlexCell class is an accessor for manipulating cells in FlexView. You can operate the pointed cell by manipulating the properties of the FlexCell.

The FlexCell object is a virtual class that underlies other accessor classes and has no substance. FlexCell-derived classes cannot be created directly from a script and are created as child objects of a FlexRow object by a method that returns FlexRow.