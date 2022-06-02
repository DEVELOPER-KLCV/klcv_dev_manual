---
layout: default

grand_parent: 2. Standard Package
parent: OptionButton Class

title: Properties
nav_order: 1
permalink: /package/standard/optionbutton/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the OptionButton class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[BgColor](/package/standard/optionbutton/properties/bgcolor) | CRW | integer | $STD  |   Background color          |
|[Border](/package/standard/optionbutton/properties/border) | CR | boolean | $FALSE  | Border display           |
|[FgColor](/package/standard/optionbutton/properties/fgcolor) | CRW | integer | $STD  |   Text color          |
|[FontFace](/package/standard/optionbutton/properties/fontface) | CR | integer | $STD  |    Font decoration properties       <br><small><span style="color:blue">There's a limit in AI</span></small>    |
|[FontKind](/package/standard/optionbutton/properties/fontkind) | CR | integer | $STD  |   Font type  <br><small><span style="color:red">Supported fonts have been added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><small><span style="color:blue">There's a limit in AI</span></small>       |
|[FontSize](/package/standard/optionbutton/properties/fontsize) | CR | integer | 10  |   Font size          |
|[Scroll](/package/standard/optionbutton/properties/scroll) | CR | integer | $AUTO  | 	Scroll bar display control <br><small><span style="color:blue">There's a limit in Mobile</span></small>  <br><small><span style="color:green">No more restriction since Mobile Ver.3.0.0</span></small>         |
|[ToolTip](/package/standard/optionbutton/properties/toolTip) | CRW | String |   |    Tooltip   <br><small><span style="color:blue">Not supported in Mobile, AI</span></small>      |
|[ToolTipDelayTime](/package/standard/optionbutton/properties/tooltipdelaytime) | CRW | integer | 0  |  Tooltip display time <br><small><span style="color:red">Added since Ver.4.2.0</span></small> <br><small><span style="color:blue">Not supported in Mobile, AI</span></small>         |
|[Value](/package/standard/optionbutton/properties/value)* | CRW | integer |   |  Selected position           |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
