---
layout: default

grand_parent: 2. Standard Package
parent: Dialog Class

title: Properties
nav_order: 1
permalink: /package/standard/dialog/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Dialog class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[BgColor](/package/standard/dialog/properties/bgcolor) | CRW | integer | $STD |Background color  |
|[Border](/package/standard/dialog/properties/border) | CR | boolean | $FALSE|Display frame |
|[CloseBox](/package/standard/dialog/properties/closebox) | CR | boolean | $TRUE|Close button active / inactive<br><small>Added since Ver.5.0.0<br>Not available in Mobile & AI</small> |
|[ControlBox](/package/standard/dialog/properties/controlbox) | CR | boolean | $TRUE|Show / hide title bar buttons<br><small>Added since Ver.5.0.0<br>Not available in Mobile & AI</small> |
|[Icon](/package/standard/dialog/properties/icon) | CRW | integer | 0|Icon number<br><small>Added since Ver.4.1.3<br>Not available in Mobile & AI</small> |
|[MaximizeBox](/package/standard/dialog/properties/maximizebox) | CR | boolean | $FALSE |Allow dialog maximization<br><small>Added since Ver.4.1.0<br>Not available in Mobile & AI</small> |
|[MinimizeBox](/package/standard/dialog/properties/minimizebox) | CR | boolean | $FALSE |Allow dialog to be minimized<br><small>Added since Ver.4.1.0<br>Not available in Mobile & AI</small> |
|[Modal](/package/standard/dialog/properties/modal) | CR | boolean | $FALSE |Specifying the modal display of the dialog<br><small>Added since Ver.5.0.4<br>Not available in Mobile & AI</small> |
|[Opacity](/package/standard/dialog/properties/opacity) |CRW | Number | 1.0 |Specifying the transparency of the dialog<br><small>Added since Ver.5.0.3<br>Not available in Mobile & AI</small> |
|[Resize](/package/standard/dialog/properties/resize) |CR | boolean | $FALSE |Allow dialog resizing<br><small>Added since Ver.4.1.0<br>Not available in Mobile & AI</small> |
|[Scroll](/package/standard/dialog/properties/scroll) |CR | integer | $AUTO |Scroll bar display control<br><small>Mobile has restriction<br>There are no restrictions since Mobile Ver.3.0.0</small> |
|[Title](/package/standard/dialog/properties/title) |CRW | String |  |Characters to be displayed in the title bar |
|[TitleBar](/package/standard/dialog/properties/titlebar) |CR | boolean | $TRUE |Show or hide the title bar<br><small>Added since Ver.5.0.3<br>Not available in Mobile & AI</small> |
|[TransparencyKey](/package/standard/dialog/properties/transparencykey) |CRW | integer | $STD |Color to apply transparency effect <br><small>Added since Ver.5.0.3<br>Not available in Mobile & AI</small>|
|[Value](/package/standard/dialog/properties/value)* |CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value<br><small>Added since Ver.4.2.0</small> |

<small>X, Y, Visible properties can be specified since Ver.4.0.0.<br>X and Y properties can now be specified from Mobile Ver.3.0.0<br>AI does not support specifying X and Y properties</small>

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property