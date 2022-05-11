---
layout: default

grand_parent: 2. Standard Package
parent: Graph Class

title: Properties
nav_order: 1
permalink: /package/standard/graph/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Graph class.

|Name       | Access | Type   |  Initial Value | Description  |
|----------	|--------|--------|----------------|--------------|
|[BgColor](/package/standard/graph/properties/bgcolor) | CRW | integer | $STD | |
|[Border](/package/standard/graph/properties/border) | CR | boolean | $FALSE | |
|[DataLabel](/package/standard/graph/properties/datalabel) | CRW | integer | $STD | |
|[Direction](/package/standard/graph/properties/direction) | CRW | integer | $VERTICAL | |
|[Example](/package/standard/graph/properties/example) | CRW | integer | $STD | |
|[FgColor](/package/standard/graph/properties/fgcolor) | CRW | integer | $STD | |
|[FontFace](/package/standard/graph/properties/fontface) | CR | integer | $STD | |
|[FontKind](/package/standard/graph/properties/fontkind) | CR | integer | $STD | |
|[FontSize](/package/standard/graph/properties/fontsize) | CR | integer | 10 | |
|[GraphType](/package/standard/graph/properties/graphtype) | CRW | integer | $BAR | |
|[Title](/package/standard/graph/properties/title) | CRW | String |  | |
|[ToolTip](/package/standard/graph/properties/tooltip) | CRW | String |  | |
|[ToolTipDelayTime](/package/standard/graph/properties/tooltipdelaytime) | CRW | integer | 0 | |
|[Value](/package/standard/graph/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property