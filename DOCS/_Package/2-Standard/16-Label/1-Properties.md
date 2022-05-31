---
layout: default

grand_parent: 2. Standard Package
parent: Label Class

title: Properties
nav_order: 1
permalink: /package/standard/label/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Label class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AcceptDrop](/package/standard/label/properties/acceptdrop) | CRW | integer | 0  | Type that accepts drag and drop<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add410.gif" alt="Image" width="50" height="12"></span></small><br><small><span style="color:blue">Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"></span></small>            |
|[BgColor](/package/standard/label/properties/bgcolor) | CRW | integer | $STD  |   Background color          |
|[Border](/package/standard/label/properties/border) | CRW | boelean | $FALSE  |   Border display          |
|[BorderStyle](/package/standard/label/properties/borderstyle) | CRW | integer | $SUNKEN  |   Border type   <br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12"></span></small><br><small><span style="color:green">Border types have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change400.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-change300.gif" alt="Image" width="86" height="12"> </span></small>      |
|[FgColor](/package/standard/label/properties/fgcolor) | CRW | integer | $STD  |    Text color         |
|[FontFace](/package/standard/label/properties/fontface) | CR | integer | $STD  | Font decoration properties <br><small><span style="color:blue"> There are limits for <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"></span></small>           |
|[FontKind](/package/standard/label/properties/fontkind) | CR | integer | $STD  |   Font type<br><small><span style="color:green">Supported fonts have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change410.gif" alt="Image" width="50" height="12"></span></small>  <br><small><span style="color:blue">Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"></span></small>  <br><small><span style="color:blue">There are limits for <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"></span></small>            |
|[FontSize](/package/standard/label/properties/fontsize) | CR | integer | 10  |  Font size           |
|[Format](/package/standard/label/properties/format) | CR | String |   |Format string   <br><small><span style="color:green">  Format that can be specified have been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change410.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-change300.gif" alt="Image" width="86" height="12"> </span></small>        |
|[HorizontalAlign](/package/standard/label/properties/horizontalalign) | CR | integer | $STD  |  Horizontal alignment           |
|[NoPrefix](/package/standard/label/properties/noprefix) | CRW | boolean | $FALSE  | Mode that does not interpret &  <br><small><span style="color:red"> Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add500.gif" alt="Image" width="50" height="12"></span></small>  <br><small><span style="color:blue"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add450.gif" alt="Image" width="86" height="12"><br>Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> </span></small>            |
|[ToolTip](/package/standard/label/properties/tooltip) | CRW | String ||Tooltip <br><small><span style="color:blue"> Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> </span></small>   |             
|[ToolTipDelayTime](/package/standard/label/properties/tooltipdelaytime) | CRW | integer | 0  | Tooltip display time<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add420.gif" alt="Image" width="50" height="12"></span></small> <br><small><span style="color:blue">Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> </span></small>            |
|[Transparent](/package/standard/label/properties/transparent) | CRW | boolean | $FALSE  |  Background transparency<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add300.gif" alt="Image" width="86" height="12"></span></small>            |
|[Value](/package/standard/label/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString | |Value to display on the label<br><small><span style="color:green">UString has been added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change420.gif" alt="Image" width="50" height="12"> </span></small> |             
|[VerticalAlign](/package/standard/label/properties/verticalalign) | CR | integer | $STD  | Vertical alignment<br><small><span style="color:green">It is also valid on the screen since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-change200.gif" alt="Image" width="86" height="12">  </span></small>           |
|[WordWrap](/package/standard/label/properties/wordwrap) | CRW | boolean | $TRUE  |Word wrap control<br><small><span style="color:red">Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add504.gif" alt="Image" width="50" height="12"></span></small> <br><small><span style="color:blue">Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-non.gif" alt="Image" width="40" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" alt="Image" width="18" height="12"> </span></small>             |

Only available for Mobile, Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[UseTapAndHold](/package/standard/label/properties/usetapandhold) | CRW | boolean | $FALSE  | Whether to use tap and hold operation  <br><small><span style="color:red"> Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add300.gif" alt="Image" width="86" height="12">   </span></small>       |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
