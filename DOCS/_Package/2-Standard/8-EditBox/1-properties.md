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
|----------	|:--------:|:--------:|:---------------:|--------------|
|[Border](/package/standard/editbox/properties/border) | CR | boolean | $TRUE|Display of frame |
|[HorizontalAlign](/package/standard/editbox/properties/horizontalalign) | CR | integer | $STD | Horizontal alignment |
|[InputMode](/package/standard/editbox/properties/inputmode) | CR | integer |  |Specifying the character types that can be entered  |
|[MaxLength](/package/standard/editbox/properties/maxlength) | CR | integer |  |Number of character bytes that can be entered (number of characters in Mobile version and Android version)  |
|[ScrollBarPosition](/package/standard/editbox/properties/scrollbarposition) | CR | integer | $STD | Display position of scroll bar |
|[Value](/package/standard/editbox/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Value to display  |
|[VerticalAlign](/package/standard/editbox/properties/verticalalign) | CR | integer | $STD | Vertical alignment (printing only) |
|[WordWrap](/package/standard/editbox/properties/wordwrap) | CR | integer | $TRUE | Word wrap control |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property