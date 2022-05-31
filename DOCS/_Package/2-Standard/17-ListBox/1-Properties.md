---
layout: default

grand_parent: 2. Standard Package
parent: ListBox Class

title: Properties
nav_order: 1
permalink: /package/standard/listbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ListBox class.


|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AcceptDrop](/package/standard/listbox/properties/acceptdrop) | CRW | integer | 0  | Type that accepts drag and drop <br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:red">Not supported in Mobile, AI</span></small>  |
|[BgColor](/package/standard/listbox/properties/bgcolor) | CRW | integer | $STD  |     Background color   <br><small><span style="color:red">Added since Ver.5.0.0, AI Ver.1.0.2</span></small><br><small><span style="color:red">Not supported in Mobile, AI</span></small>      |
|[Border](/package/standard/listbox/properties/border) | CR | boelean | $FALSE  |   Display border          |
|[FgColor](/package/standard/listbox/properties/fgcolor) | CRW | integer | $STD  |     Text color <br><small><span style="color:red">Added since Ver.5.0.0, AI Ver.1.0.2</span></small><br><small><span style="color:red">Not supported in Mobile, AI</span></small>       |
|[FontFace](/package/standard/listbox/properties/fontface) | CR | integer | $STD  |    Font decoration properties         |
|[FontKind](/package/standard/listbox/properties/fontkind) | CR | integer | $STD  |   Font type <br><small><span style="color:green">Supported fonts have been added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><small><span style="color:blue">There's a limit in AI</span></small>         |
|[FontSize](/package/standard/listbox/properties/fontsize) | CR | integer | 10  |  font size           |
|[Scroll](/package/standard/listbox/properties/scroll) | CR | integer | $AUTO | 	Scroll bar display control <br><small><span style="color:blue">There's a limit in Mobile</span></small><br><small><span style="color:green">No more restriction since Mobile Ver.3.0.0</span></small>|
|[SelectionMode](/package/standard/listbox/properties/selectionmode) | CRW | String | | Selection mode |
|[ToolTip](/package/standard/listbox/properties/tooltip) | CRW | String |   |  Tooltip   <br><small><span style="color:blue">Not supported in Mobile, AI</span></small>         |
|[ToolTipDelayTime](/package/standard/listbox/properties/tooltipdelaytime) | CRW | integer | 0  |  Tooltip display time    <br><small><span style="color:red">Added since Ver.4.2.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>  |
|[Value](/package/standard/listbox/properties/value)* | CRW | integer |   |   	Selected position          |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property 
