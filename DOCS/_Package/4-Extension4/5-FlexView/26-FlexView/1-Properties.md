---
layout: default

grand_parent: FlexView Class
parent: FlexView Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexview/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexView class.

|Name      | Access | Type   |Initial Value | Description |
|----------	|--------|--------|---------------|-----------|
|[AcceptDrop](/package/extension4/flexview/flexview/properties/acceptdrop) | CRW | integer |  0 | Type that accepts drag and drop <br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[BgColor](/package/extension4/flexview/flexview/properties/bgcolor) | CRW | integer |  0 |Background color |
|[Border](/package/extension4/flexview/flexview/properties/border) | CR | boolean |  $FALSE |Display frame |
|[ColumnPosition](/package/extension4/flexview/flexview/properties/columnposition) | CRW | integer |  -1 |Cursor column |
|[CursorCellOpacity](/package/extension4/flexview/flexview/properties/cursorcellopacity) | CRW | integer |  0 |Cursor transparency in cursor cell |
|[CursorColor](/package/extension4/flexview/flexview/properties/cursorcolor) | CRW | integer |  0 | Cursor color|
|[CursorLineOpacity](/package/extension4/flexview/flexview/properties/cursorlineopacity) | CRW | integer |  100 | Cursor transparency of cursor row|
|[CursorMove](/package/extension4/flexview/flexview/properties/cursormove) | CRW | integer |  $STD |How to move the cursor <br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">There's a limit in Mobile, AI</span></small> |
|[CursorTextColor](/package/extension4/flexview/flexview/properties/cursortextcolor) | CRW | integer |  0 | Text color of cursor cell|
|[FontFace](/package/extension4/flexview/flexview/properties/fontface) | CR | integer |  $STD | Font decoration attributes<br><small><span style="color:blue">There's a limit in AI</span></small>|
|[FontKind](/package/extension4/flexview/flexview/properties/fontkind) | CR | integer |  $STD |Font type <br><small><span style="color:green">Supported fonts have been added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><small><span style="color:blue">There's a limit in AI</span></small> |
|[FontSize](/package/extension4/flexview/flexview/properties/fontsize) | CR | integer |  10 | Font size |
|[HScroll](/package/extension4/flexview/flexview/properties/hscroll) | CR | integer |  $AUTO |How to display the horizontal scroll bar |
|[NoPrefix](/package/extension4/flexview/flexview/properties/noprefix) | CRW | boolean |  $FALSE |Mode without interpretation of & <br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small> |
|[RowCount](/package/extension4/flexview/flexview/properties/rowcount) | CR | integer |  0 | Current number of rows|
|[RowPosition](/package/extension4/flexview/flexview/properties/rowposition) | CRW | integer |  -1 | Cursor row|
|[ShowTitle](/package/extension4/flexview/flexview/properties/showtitle) | CRW | boolean |  $TRUE |Title display control |
|[TitleBgColor](/package/extension4/flexview/flexview/properties/titlebgcolor) | CRW | integer |  0 | Title background color|
|[TitleFgColor](/package/extension4/flexview/flexview/properties/titlefgcolor) | CRW | integer |  0 | Title text color|
|[TitleFontFace](/package/extension4/flexview/flexview/properties/titlefontface) | CR | integer |  $STD | Title font decoration attributes<br><small><span style="color:red">Added since Ver.5.0.2</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[TitleFontKind](/package/extension4/flexview/flexview/properties/titlefontkind) | CR | integer |  $STD |<br><small><span style="color:red">Added since Ver.5.0.2</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[TitleFontSize](/package/extension4/flexview/flexview/properties/titlefontsize) | CR | integer |  $STD | <br><small><span style="color:red">Added since Ver.5.0.2</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[TitleHeight](/package/extension4/flexview/flexview/properties/titleheight) | CRW | integer |  20 | |
|[TooTipDelayTime](/package/extension4/flexview/flexview/properties/tooltipdelaytime) | CRW | integer |  0 |<br><small><span style="color:red">Added since Ver.4.2.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[UseTitleFont](/package/extension4/flexview/flexview/properties/usetitlefont) | CR | boolean |  $FALSE | <br><small><span style="color:red">Added since Ver.5.0.2</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[VScroll](/package/extension4/flexview/flexview/properties/vscroll) | CR | integer |  $AUTO | How to display the vertical scroll bar|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property