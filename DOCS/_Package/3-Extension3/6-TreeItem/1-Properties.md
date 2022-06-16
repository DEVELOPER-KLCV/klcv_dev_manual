---
layout: default

grand_parent: 3. Extension3 Package
parent: TreeItem Class

title: Properties
nav_order: 1
permalink: /package/extension3/treeitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TreeItem class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[CloseIcon](/package/extension3/treeitem/properties/closeicon) | CR | integer |  |Tree closed icon |
|[Expanded](/package/extension3/treeitem/properties/expanded) | CRW | boolean | $FALSE |Expand/Collapse state of the tree item |
|[OpenIcon](/package/extension3/treeitem/properties/openicon) | CR | integer |  | Tree open icon|
|[Title](/package/extension3/treeitem/properties/title) | CRW | String |  | Characters to display on tree items|
|[Value](/package/extension3/treeitem/properties/value) | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value<br> <small><span style="color:green">UString have been added since Ver.4.2.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
