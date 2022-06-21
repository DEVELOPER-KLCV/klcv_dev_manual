---
layout: default

grand_parent: FlexView Class
parent: FlexGroupHeader Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexgroupheader/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexGroupHeader class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[GroupCount](/package/extension4/flexview/flexgroupheader/properties/groupcount) | CRW | integer | 0 |Group unit |
|[HorizontalAlign](/package/extension4/flexview/flexgroupheader/properties/horizontalalign) | CR | integer | $STD |Horizontal alignment |
|[Value](/package/extension4/flexview/flexgroupheader/properties/value)* | CRW  |String<br>Number<br>Fixed<br>Date<br>UString |  |Initial cell value <br><small><span style="color:green">UString have been added since Ver.4.2.0</span></small>|

※Depends on the ValueType of the inherited class

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property