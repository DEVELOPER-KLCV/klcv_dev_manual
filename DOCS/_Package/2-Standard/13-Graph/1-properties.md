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
|[BgColor](/package/standard/graph/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/standard/graph/properties/border) | CR | boolean | $FALSE | Frame display |
|[DataLabel](/package/standard/graph/properties/datalabel) | CRW | integer | $STD | Data label display method|
|[Direction](/package/standard/graph/properties/direction) | CRW | integer | $VERTICAL |Graph direction |
|[Example](/package/standard/graph/properties/example) | CRW | integer | $STD | Graph legend display method |
|[FgColor](/package/standard/graph/properties/fgcolor) | CRW | integer | $STD | Font color |
|[FontFace](/package/standard/graph/properties/fontface) | CR | integer | $STD | Font decoration properties|
|[FontKind](/package/standard/graph/properties/fontkind) | CR | integer | $STD | Font type <br><small><span style="color:red">Supported fonts have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"></span></small> |
|[FontSize](/package/standard/graph/properties/fontsize) | CR | integer | 10 | Font size |
|[GraphType](/package/standard/graph/properties/graphtype) | CRW | integer | $BAR | Graph type|
|[Title](/package/standard/graph/properties/title) | CRW | String |  | Title text |
|[ToolTip](/package/standard/graph/properties/tooltip) | CRW | String |  | Tool tip|
|[ToolTipDelayTime](/package/standard/graph/properties/tooltipdelaytime) | CRW | integer | 0 | Tool tip display time <br><small><span style="color:red">Supported fonts have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add420.gif" alt="Image" width="50" height="12"></span></small>|
|[Value](/package/standard/graph/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  | Object value |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property