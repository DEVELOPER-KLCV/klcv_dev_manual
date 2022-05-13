---
layout: default

grand_parent: 2. Standard Package
parent: DisplayObject Class

title: Properties
nav_order: 1
permalink: /package/standard/displayobject/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the DisplayObject class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[Active](/package/standard/displayobject/properties/active) | CRW | boolean | $TRUE |Control of activity  |
|[Height](/package/standard/displayobject/properties/height) | CRW | integer | 100 |Vertical display size  |
|[MouseOperation](/package/standard/displayobject/properties/mouseoperation) | CRW | integer | $STD |Specification regarding mouse operation<br>Added since  Ver.5.0.3<br> Not available in Mobile & AI</small> |
|[TabIndex](/package/standard/displayobject/properties/tabindex) | CR | integer | 32767 |Display and input priority  |
|[Visible](/package/standard/displayobject/properties/visible) | CRW | boolean | $TRUE |Display control  |
|[VisualStyle](/package/standard/displayobject/properties/visualstyle) | CR | boolean | $TRUE |Visual style ON / OFF <br>Added since  Ver.5.0.0<br> Not available in Mobile & AI</small> |
|[Width](/package/standard/displayobject/properties/width) | CRW | integer | 100 |Horizontal display size  |
|[X](/package/standard/displayobject/properties/x) | CRW | integer | 0 | Horizontal display position <br><small>Also enabled for Form directly under AI Ver.1.0.2 Root</small> |
|[Y](/package/standard/displayobject/properties/y) | CRW | integer | 0 | Horizontal display position<br><small>Also enabled for Form directly under AI Ver.1.0.2 Root</small>  |


Properties added only to array objects

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[Layout](/package/standard/displayobject/properties/layout) | CR | integer | $VERTICAL |Layout when arrayed<br> <small>Added Ver.5.0.0, Mobile Ver.4.5.0 $ OPTIMAL<br>($ HORIZONTAL and optimized placement according to the label string length)</small>  |
|[LayoutMargin](/package/standard/displayobject/properties/layoutmargin) | CR | integer | 0 |Interval when arranging  |
|[LayoutSpacing](/package/standard/displayobject/properties/layoutspacing) | CR | integer | 0 |Margins when arranging  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable