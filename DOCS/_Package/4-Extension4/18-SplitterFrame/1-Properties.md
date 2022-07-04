---
layout: default

grand_parent: 4. Extension4 Package
parent: SplitterFrame Class

title: Properties
nav_order: 1
permalink: /package/extension4/splitterframe/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the SplitterFrame class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[BgColor](/package/extension4/splitterframe/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/extension4/splitterframe/properties/border) | CR | boolean | $FALSE | Frame display|
|[MaxPosition](/package/extension4/splitterframe/properties/maxposition) | CRW | integer | 0 |Maximum value of the controllable range of the split line |
|[MinPosition](/package/extension4/splitterframe/properties/minposition) | CRW | integer | 0 | Minimum value of the controllable range of the split line|
|[Resize](/package/extension4/splitterframe/properties/resize) | CRW | boolean | $TRUE |Whether the position of the split line can be changed |
|[SplitDirection](/package/extension4/splitterframe/properties/splitdirection) | CR | integer | $VERTICAL | Split direction|
|[SplitPolicy](/package/extension4/splitterframe/properties/splitpolicy) | CR | integer | $ABSOLUTE | SplitPosition property unit|
|[SplitPosition](/package/extension4/splitterframe/properties/splitposition) | CRW | integer | 40 |split line position |
|[ThumbColor](/package/extension4/splitterframe/properties/thumbcolor) | CR | integer | $STD |Split line color |
|[ThumbSize](/package/extension4/splitterframe/properties/thumbsize) | CR | integer | 2 | Split line thickness|
|[ThumbStyle](/package/extension4/splitterframe/properties/thumbstyle) | CR | integer | $STD | Split line appearance |
|[Value](/package/extension4/splitterframe/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value <br><small><span style="color:green">Added UString since Ver.4.2.0</span></small> |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property