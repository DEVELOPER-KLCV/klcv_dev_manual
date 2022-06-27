---
layout: default

grand_parent: 4. Extension4 Package
parent: ImageButton Class

title: Properties
nav_order: 1
permalink: /package/extension4/imagebutton/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ImageButton class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[BgColor](/package/extension4/imagebutton/properties/bgcolor) | CRW | integer | $STD |Background color  |
|[Border](/package/extension4/imagebutton/properties/border) | CR | boolean | $TRUE |Frame display <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[ButtonMode](/package/extension4/imagebutton/properties/buttonmode) | CRW | integer | $PUSH | Button operation mode  |
|[ButtonStyle](/package/extension4/imagebutton/properties/buttonstyle) | CRW | integer | $STD | Background color when inactive <br><small><span style="color:green">Specifiable values have been added from Ver.5.0.3.</span></small> |
|[DisabledBgColor](/package/extension4/imagebutton/properties/disabledbgcolor) | CRW | integer | $STD | Background color when inactive<br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>  |
|[DisabledFgColor](/package/extension4/imagebutton/properties/disabledfgcolor) | CRW | integer | $STD |Text color when inactive  |
|[FgColor](/package/extension4/imagebutton/properties/fgcolor) | CRW | integer | $STD | Text color |
|[FocusRect](/package/extension4/imagebutton/properties/focusrect) | CRW | boolean | $TRUE | Whether to display a rectangular dotted line that indicates focus <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[HorzPlacement](/package/extension4/imagebutton/properties/horzplacement) | CRW | integer | $STD | Horizontal display position of images and characters |
|[HoveredBgColor](/package/extension4/imagebutton/properties/hoveredbgcolor) | CRW | integer | $STD | Background color when mouse cursor is over button <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[HoveredFgColor](/package/extension4/imagebutton/properties/hoveredfgcolor) | CRW | integer | $STD |Text color when mouse cursor is over button <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[ImageHeight](/package/extension4/imagebutton/properties/imageheight) | CRW | integer | 32 |Height when enlarging / reducing the image  |
|[ImageWidth](/package/extension4/imagebutton/properties/imagewidth) | CRW | integer | 32 |Width when enlarging / reducing the image  |
|[NoAutoPadding](/package/extension4/imagebutton/properties/noautopadding) | CRW | boolean | $FALSE |Whether to automatically adjust the spacing between the image and the text <br><small><span style="color:red">Added since Ver.5.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[NoPrefix](/package/extension4/imagebutton/properties/noprefix) | CRW | boolean | $FALSE | Mode without interpretation of &  <br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small>|
|[PushedBgColor](/package/extension4/imagebutton/properties/pushedbgcolor) | CRW | integer | $STD | Background color when pressed <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[PushedFgColor](/package/extension4/imagebutton/properties/pushedfgcolor) | CRW | integer | $STD |Text color when pressed <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[PushingBgColor](/package/extension4/imagebutton/properties/pushingbgcolor) | CRW | integer | $STD |Background color while pressed in toggle mode <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[PushingFgColor](/package/extension4/imagebutton/properties/pushingfgcolor) | CRW | integer | $STD | Text color while pressed in toggle mode <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[Resize](/package/extension4/imagebutton/properties/resize) | CRW | integer | $STD | How to enlarge / reduce the image |
|[Spacing](/package/extension4/imagebutton/properties/spacing) | CRW | integer | 5 | Peripheral margin |
|[TextAlign](/package/extension4/imagebutton/properties/textalign) | CRW | integer | $STD | Display position within the text display area <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[TextHOffset](/package/extension4/imagebutton/properties/texthoffset) | CRW | integer | 0 |Adjusting the text display position horizontally <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[TextVOffset](/package/extension4/imagebutton/properties/textvoffset) | CRW | integer | 0 | Adjusting the text display position vertically <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Toggle](/package/extension4/imagebutton/properties/toggle) | CRW | integer | 0 |Toggle button state  |
|[VerticalAlign](/package/extension4/imagebutton/properties/verticalalign) | CR | integer | $STD | Vertical alignment |
|[VertPlacement](/package/extension4/imagebutton/properties/vertplacement) | CRW | integer | $STD |Vertical display position of image and text  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable