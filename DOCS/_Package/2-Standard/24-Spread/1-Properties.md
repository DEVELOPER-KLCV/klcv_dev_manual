---
layout: default

grand_parent: 2. Standard Package
parent: Spread Class

title: Properties
nav_order: 1
permalink: /package/standard/spread/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Spread class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AcceptDrop](/package/standard/spread/properties/acceptdrop) | CRW | integer | 0 | Type that accepts drag and drop <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"></span></small>|
|[BgColor](/package/standard/spread/properties/bgcolor) | CRW | integer | $STD | Background color|
|[Border](/package/standard/spread/properties/border) | CR | boolean | $FALSE |Display of frame |
|[ColumnPosition](/package/standard/spread/properties/columnPosition) | CRW | integer |  | Selected column number|
|[CursorColor](/package/standard/spread/properties/cursorcolor) | CRW | integer |  | Cursor color|
|[FgColor](/package/standard/spread/properties/fgcolor) | CRW | integer | $STD |Text color |
|[FontFace](/package/standard/spread/properties/fontface) | CR | integer | $STD | Font decoration attributes|
|[FontKind](/package/standard/spread/properties/fontkind) | CR | integer | $STD | Font type <br><small><span style="color:red">Supported font have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"></span></small>|
|[FontSize](/package/standard/spread/properties/fontsize) | CR | integer | 10 |Font size |
|[HorizontalAlign](/package/standard/spread/properties/horizontalAlign) | CR | integer | $STD |(Doesn't work, left for compatibility.) |
|[HScroll](/package/standard/spread/properties/hscroll) | CR | integer | $AUTO | How to display the horizontal scroll bar|
|[NumberBgColor](/package/standard/spread/properties/numberbgcolor) | CR | integer | $STD | Row header background color |
|[NumberColor](/package/standard/spread/properties/numbercolor) | CRW | integer | $STD | Line header display color|
|[LabelBgColor](/package/standard/spread/properties/labelbgcolor) | CRW | integer | $STD |Column header background color |
|[LabelColor](/package/standard/spread/properties/labelcolor) | CRW | integer | $STD | Column header display color|
|[LockColumns](/package/standard/spread/properties/lockcolumns) | CRW | integer | 0 | Number of fixed columns <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add403.gif" alt="Image" width="50" height="12"></span></small>|
|[RowLabelMode](/package/standard/spread/properties/rowlabelmode) | CRW | integer |  |	Row header display mode<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add400.gif" alt="Image" width="50" height="12"></span></small> |
|[RowLabelWidth](/package/standard/spread/properties/rowlabelwidth) | CRW | integer |  | Line header display width <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add400.gif" alt="Image" width="50" height="12"></span></small> |
|[SelectionMode](/package/standard/spread/properties/selectionMode) | CR | integer | $STD |Selection mode |
|[ShowLabel](/package/standard/spread/properties/showlabel) | CRW | boolean | $TRUE | Column header display control|
|[ShowNumber](/package/standard/spread/properties/shownumber) | CRW | boolean | $TRUE | Row header display control|
|[ToolTip](/package/standard/spread/properties/tooltip) | CRW | String |  | Tooltip |
|[ToolTipDelayTime](/package/standard/spread/properties/tooltipdelaytime) | CRW | integer | 0 | Tooltip display time <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add420.gif" alt="Image" width="50" height="12"></span></small> |
|[Value](/package/standard/spread/properties/value)* | CRW | integer |  |Selected line number |
|[VScroll](/package/standard/spread/properties/vscroll) | CR | integer | $AUTO | How to display the vertical scroll bar|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
