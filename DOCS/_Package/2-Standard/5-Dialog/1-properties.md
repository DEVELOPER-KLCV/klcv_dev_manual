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
|[BgColor](/package/standard/dialog/properties/bgcolor) | CRW | integer | $STD |  |
|[Border](/package/standard/dialog/properties/border) | CR | boolean | $FALSE| |
|[CloseBox](/package/standard/dialog/properties/closebox) | CR | boolean | $TRUE| |
|[ControlBox](/package/standard/dialog/properties/controlbox) | CR | boolean | $TRUE| |
|[Icon](/package/standard/dialog/properties/icon) | CRW | integer | 0| |
|[MaximizeBox](/package/standard/dialog/properties/maximizebox) | CR | boolean | $FALSE | |
|[MinimizeBox](/package/standard/dialog/properties/minimizebox) | CR | boolean | $FALSE | |
|[Modal](/package/standard/dialog/properties/modal) | CR | boolean | $FALSE | |
|[Opacity](/package/standard/dialog/properties/opacity) |CRW | Number | 1.0 | |
|[Resize](/package/standard/dialog/properties/eesize) |CR | boolean | $FALSE | |
|[Scroll](/package/standard/dialog/properties/scroll) |CR | integer | $AUTO | |
|[Title](/package/standard/dialog/properties/title) |CRW | String |  | |
|[TitleBar](/package/standard/dialog/properties/titlebar) |CR | boolean | $TRUE | |
|[TransparencyKey](/package/standard/dialog/properties/transparencykey) |CRW | integer | $STD | |
|[Value](/package/standard/dialog/properties/value)* |CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |



<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property