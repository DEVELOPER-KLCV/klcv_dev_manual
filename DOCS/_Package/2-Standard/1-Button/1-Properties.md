---
layout: default

grand_parent: 2. Standard Package
parent: Button Class

title: Properties
nav_order: 1
permalink: /package/standard/button/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Button class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|
|[AltKey](/package/standard/button/properties/altkey) | CR | integer | $STD |Alternate key to raise the Touch event |
|[FontFace](/package/standard/button/properties/fontface) | CR | integer | $STD |Font decoration attributes <br> <small>AI has restrictions</small> |
|[FontKind](/package/standard/button/properties/fontkind) | CR | integer | $STD |	Font type<br><small>Supported fonts have been added since Ver.4.1.0<br>Not supported on Mobile<br>AI has restrictions</small> |
|[FontSize](/package/standard/button/properties/fontsize) | CR | integer | 10 |Font size |
|[HorizontalAlign](/package/standard/button/properties/horizontalAlign) | CR | integer | 10 |Horizontal alignment |
|[Title](/package/standard/button/properties/title) | CRW | String<br>UString(※) | | Character to be displayed on the button<br> ( ※ ) When ValueType is UString <br><small>Added since Ver.5.0.3</small> |
|[Tooltip](/package/standard/button/properties/tooltip) | CRW | String |  |Tooltip <br><small>Not supported on Mobile</small>|
|[ToolTipDelayTime](/package/standard/button/properties/tooltipdelaytime) | CRW | integer | 0 |Tooltip display time<br><small>Added since Ver.4.2.0<br>Not supported on Mobile</small> |
|[Value](/package/standard/button/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value<br><small>UString has been added since Ver.4.2.0</small> |
|[VerticalAlign](/package/standard/button/properties/verticalAlign) | CR | integer | $STD |Vertical alignment (printing only)<br><small>Not supported on Mobile</small> |
|[AltKey](/package/standard/button/properties/altkey) | CR | integer | $STD | |
|[FontFace](/package/standard/button/properties/fontface) | CR | integer | $STD | |
|[FontKind](/package/standard/button/properties/fontkind) | CR | integer | $STD | |
|[FontSize](/package/standard/button/properties/fontsize) | CR | integer | 10 | |
|[HorizontalAlign](/package/standard/button/properties/horizontalalign) | CR | integer | 10 | |
|[Title](/package/standard/button/properties/title) | CRW | String<br>UString(※) |  | |
|[Tooltip](/package/standard/button/properties/tooltip) | CRW | String |  | |
|[ToolTipDelayTime](/package/standard/button/properties/tooltipdelaytime) | CRW | integer | 0 | |
|[Value](/package/standard/button/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |
|[VerticalAlign](/package/standard/button/properties/verticalalign) | CR | integer | $STD | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property