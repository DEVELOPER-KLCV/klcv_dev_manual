---
layout: default

grand_parent: 1. Standard Package
parent: Button

title: Properties
nav_order: 1
permalink: /package/standard/button/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Button class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[AltKey](/package/standard/button/properties/length) | CR | integer | $STD | |
|[FontFace](/package/standard/button/properties/fontface) | CR | integer | $STD | |
|[FontKind](/package/standard/button/properties/fontkind) | CR | integer | $STD | |
|[FontSize](/package/standard/button/properties/fontsize) | CR | integer | 10 | |
|[HorizontalAlign](/package/standard/button/properties/horizontalAlign) | CR | integer | 10 | |
|[Title](/package/standard/button/properties/title) | CRW | String<br>UString(※) |  | |
|[Tooltip](/package/standard/button/properties/tooltip) | CRW | String |  | |
|[ToolTipDelayTime](/package/standard/button/properties/tooltipdelaytime) | CRW | integer | 0 | |
|[Value](/package/standard/button/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |
|[VerticalAlign](/package/standard/button/properties/verticalAlign)* | CR | integer | $STD | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property