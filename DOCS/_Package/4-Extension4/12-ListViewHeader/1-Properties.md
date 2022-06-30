---
layout: default

grand_parent: 4. Extension4 Package
parent: ListViewHeader Class

title: Properties
nav_order: 1
permalink: /package/extension4/listviewheader/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ListViewHeader class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[ColHorzAlign](/package/extension4/listviewheader/properties/colhorzalign) | CR | integer | $STD |<br><small><span style="color:green">It also affects the placement of column names since Ver.5.0.0.</span></small> |
|[HorizontalAlign](/package/extension4/listviewheader/properties/horizontalign) | CR | integer | $STD | <br><small><span style="color:green">It also affects the placement of column names since Ver.5.0.0.</span></small>|
|[Title](/package/extension4/listviewheader/properties/title) | CRW | String |  | Column name|
|[Value](/package/extension4/listviewheader/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  | Object value|
|[Visible](/package/extension4/listviewheader/properties/visible) | CRW | boolean | $TRUE |Display/Hide |
|[Width](/package/extension4/listviewheader/properties/width) | CRW | integer | 100 | Column width|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property 