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
|[BgColor](/package/standard/dialog/properties/BgColor) | CRW | integer | $STD |  |
|[Border](/package/standard/dialog/properties/border) | CR | boolean | $FALSE| |
|[CloseBox](/package/standard/dialog/properties/closebox) | CR | boolean | $TRUE| |
|[ControlBox](/package/standard/dialog/properties/ControlBox) | CR | boolean | $TRUE| |
|[Icon](/package/standard/dialog/properties/Icon) | CRW | integer | 0| |
|[MaximizeBox](/package/standard/dialog/properties/MaximizeBox) | CR | boolean | $FALSE | |
|[MinimizeBox](/package/standard/dialog/properties/MinimizeBox) | CR | boolean | $FALSE | |
|[Modal](/package/standard/dialog/properties/Modal) | CR | boolean | $FALSE | |
|[Opacity](/package/standard/dialog/properties/Opacity) |CRW | Number | 1.0 | |
|[Resize](/package/standard/dialog/properties/Resize) |CR | boolean | $FALSE | |
|[Scroll](/package/standard/dialog/properties/Scroll) |CR | integer | $AUTO | |
|[Title](/package/standard/dialog/properties/Title) |CRW | String |  | |
|[TitleBar](/package/standard/dialog/properties/TitleBar) |CR | boolean | $TRUE | |
|[TransparencyKey](/package/standard/dialog/properties/TransparencyKey) |CRW | integer | $STD | |
|[Value](/package/standard/dialog/properties/value)* |CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | |



<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property