---
layout: default

grand_parent: 2. Standard Package
parent: EditObject Class

title: Properties
nav_order: 1
permalink: /package/standard/editobject/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the EditObject class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[AcceptDrop](/package/standard/editobject/properties/acceptdrop) | CRW | integer | 0 | Type that accepts drag and drop<br> <small>Added since Ver.4.1.0 <br> Not supported in Mobile, AI</small>|
|[BgColor](/package/standard/editobject/properties/bgcolor) | CRW | integer | $STD | Background color |
|[Copyable](/package/standard/editobject/properties/copyable) | CRW | boolean | $TRUE |	Copyability<br><small>Added since Ver.5.0.0 <br> Not supported in Mobile, AI</small>  |
|[Editable](/package/standard/editobject/properties/editable) | CRW | boolean | $TRUE |	Editability  |
|[FgColor](/package/standard/editobject/properties/fgcolor) | CRW | integer | $STD | Text color  |
|[FontFace](/package/standard/editobject/properties/fontface) | CR | integer | $STD | Font decoration attributes <br><small>There are limits in AI</small> |
|[FontKind](/package/standard/editobject/properties/fontkind) | CR | integer | $STD | Font type <br><small>Supported fonts have been added from Ver4.1.0</small> <br><small>There are limits in AI</small><br><small>Not supported in Mobile</small>|
|[FontSize](/package/standard/editobject/properties/fontsize) | CR | integer | 10 | font size |
|[IMECodeInput](/package/standard/editobject/properties/imecodeinput) | CR | boolean | $FALSE | Use of IME character code input extension <br><small>Added since Ver.4.2.0</small><br><small>It is always disabled on Windows Vista or later version, since Ver.5.0.2</small><br><small>There are limits in AI</small><br><small>Not supported in Mobile</small>|
|[IMEMode](/package/standard/editobject/properties/imemode) | CR | integer | $STD | Specifying IME mode |
|[IMEZoomRatio](/package/standard/editobject/properties/imezoomratio) | CR | integer | 0 |Using the IME conversion string enlargement <br> <small>Added since Ver.4.2.0 <br> Not supported in Mobile, AI</small>  |
|[SelectAllOnFocus](/package/standard/editobject/properties/selectallonfocus) | CR | integer | $STD | Specifying the selected state when receiving focus<br><small>Added since Ver.5.0.3 <br><small> Not supported in Mobile, AI</small> |
|[ShowCaret](/package/standard/editobject/properties/showcaret) | CR | boolean | $TRUE |Show / hide caret<br><small>Added since Ver.5.0.3 <br> Not supported in Mobile, AI</small>  |
|[ToolTip](/package/standard/editobject/properties/tooltip) | CRW | String | $STD | Tooltip<br><small> Not supported in Mobile, AI</small> |
|[ToolTipDelayTime](/package/standard/editobject/properties/tooltipdelaytime) | CRW | integer | 0 | Tooltip display time <small>Added since Ver.4.2.0<br> Not supported in Mobile, AI</small>|


Only for Mobile and Android version

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[UseTapAndHold](/package/standard/editobject/properties/usetapandhold) | CRW | boolean | $FALSE |Whether to use tap and hold operation<br><small>Added since Mobile Ver.3.0.0</small>  |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable