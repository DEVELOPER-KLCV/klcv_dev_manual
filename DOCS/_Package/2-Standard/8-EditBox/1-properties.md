---
layout: default

grand_parent: 2. Standard Package
parent: EditBox Class

title: Properties
nav_order: 1
permalink: /package/standard/editbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the EditBox class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[Border](/package/standard/editbox/properties/border) | CR | boolean | $TRUE |  |
|[HorizontalAlign](/package/standard/editbox/properties/horizontalalign) | CR | integer | $STD |  |
|[InputMode](/package/standard/editbox/properties/inputmode) | CR | integer |  |  |
|[MaxLength](/package/standard/editbox/properties/maxlength) | CR | integer |  |  |
|[ScrollBarPosition](/package/standard/editbox/properties/scrollbarposition) | CR | integer | $STD |  |
|[Value](/package/standard/editbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |  |
|[VerticalAlign](/package/standard/editbox/properties/verticalalign) | CR | integer | $STD |  |
|[WordWrap](/package/standard/editbox/properties/wordwrap) | CR | integer | $TRUE |  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property