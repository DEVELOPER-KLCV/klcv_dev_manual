---
layout: default

grand_parent: 4. Extension4 Package
parent: TextFrame Class

title: Properties
nav_order: 1
permalink: /package/extension4/textframe/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the TextFrame class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[Border](/package/extension4/textframe/properties/border) | CR | boolean | $TRUE | |
|[Editable](/package/extension4/textframe/properties/editable) | R | boolean | $FALSE | |
|[HorizontalAlign](/package/extension4/textframe/properties/horizontalalign) | CR | integer | $STD | |
|[ScrollBarPosition](/package/extension4/textframe/properties/scrollbarposition) | CR | integer | $STD | |
|[Value](/package/extension4/textframe/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |
|[VerticalAlign](/package/extension4/textframe/properties/verticalalign) | CR | integer | $STD | |
|[WordWrap](/package/extension4/textframe/properties/wordwrap) | CR | integer | $TRUE | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property