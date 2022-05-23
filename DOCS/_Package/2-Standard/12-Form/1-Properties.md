---
layout: default

grand_parent: 2. Standard Package
parent: Form Class

title: Properties
nav_order: 1
permalink: /package/standard/form/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Form class.

|Name       | Access | Type   |  Initial Value | Description  |
|----------	|--------|--------|----------------|--------------|
|[AcceptDrop](/package/standard/form/properties/acceptdrop) | CRW | integer | 0  |Type that accepts drag and drop<br><small><span style="color:red">Added since Ver.4.0.1</span><br> <span style="color:blue"> Not supported in Mobile, AI</span></small> |
|[BgColor](/package/standard/form/properties/bgcolor) | CRW | integer | $STD |	Background color |
|[BgHighQuality](/package/standard/form/properties/bghighquality) | CRW | boolean | $FALSE |Background display quality <small><span style="color:blue"> Not supported in Mobile, AI</span></small>|
|[BgPattern](/package/standard/form/properties/bgpattern) | CRW | XmlDocument| |SVG to display in the background of the form<br><small><span style="color:blue"> Not supported in Mobile, AI</span></small>  |
|[BgPatternCache](/package/standard/form/properties/bgpatterncache) | CRW | boolean | $FALSE |Cache with background SVG as an image<br><small><span style="color:red">Added since Ver.4.0.1</span><br> <span style="color:blue"> Not supported in Mobile, AI</span></small> |
|[Border](/package/standard/form/properties/border) | CR | boolean | $FALSE |Display of frame|
|[FontScale](/package/standard/form/properties/fontscale) | CRW | Number | 1.0 | Font scaling ratio<br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small>  |
|[HorizontalScale](/package/standard/form/properties/horizontalscale) | CRW | Number | 1.0 | Horizontal enlargement / reduction rate<br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small>  |
|[Scroll](/package/standard/form/properties/scroll) | CR | integer | $AUTO | Scroll bar display control <br><small><span style="color:blue">There are limits in Mobile</span><br><span style="color:green">No more restrictions since Mobile Ver.3.0.0</span></small> |
|[Transparent](/package/standard/form/properties/transparent) | CR | boolean | $FALSE | Background transparency <br><small><span style="color:red">Added since Ver.5.0.4</span><br> <span style="color:blue"> Not supported in Mobile, AI</span></small>  |
|[UseGesture](/package/standard/form/properties/usegesture) | CRW | integer | $STD | Specifying the gesture event to capture<br><small><span style="color:red">Added since Ver.5.0.4</span><br> <span style="color:blue"> Not supported in Mobile, AI</span></small> |
|[UseMouseMove](/package/standard/form/properties/usemousemove) | CRW | integer | $STD | Conditions for generating MouseMove events <br> <small><span style="color:blue"> Not supported in AI</span></small> |
|[UseMouseWheel](/package/standard/form/properties/usemousewheel) | CRW | integer | $STD | 	Conditions for generating MouseWheel events <br><small><span style="color:red">Added since Ver.5.0.0</span><br> <span style="color:blue"> Not supported in Mobile, AI</span></small>  |
|[Value](/package/standard/form/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |  Object value<br><small><span style="color:green">UString has been added from Ver.4.2.0</span></small>   |
|[VerticalScale](/package/standard/form/properties/verticalscale) | CRW | Number | 1.0 | Vertical scaling ratio <br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small>   |

Only for Mobile, Android version

|Name       | Access | Type   |  Initial Value | Description  |
|----------	|--------|--------|----------------|--------------|
|[usetapandhold](/package/standard/form/properties/UseTapAndHold) | CRW | boolean | $FALSE  | Whether to use tap and hold operation <br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property