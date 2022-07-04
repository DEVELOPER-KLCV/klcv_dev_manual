---
layout: default

grand_parent: 4. Extension4 Package
parent: ProgressBar Class

title: Properties
nav_order: 1
permalink: /package/extension4/progressbar/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ProgressBar class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[AutoClose](/package/extension4/progressbar/properties/autoclose) | CR | boolean | $TRUE | Whether to automatically close the pop-up window|
|[BarColor](/package/extension4/progressbar/properties/barcolor) | CRW | integer | $STD | Progress bar color|
|[BarStyle](/package/extension4/progressbar/properties/barstyle) | CR | integer | $BLOCK |Progress bar type |
|[BgColor](/package/extension4/progressbar/properties/bgcolor) | CRW | integer | $STD |Progress bar background color |
|[Border](/package/extension4/progressbar/properties/border) | CR | boolean | $FALSE  |Display frame |
|[CancelCaption](/package/extension4/progressbar/properties/cancelcaption) | CRW | String |  |Title of the cancel button of the window that pops up<br><small><span style="color:red">Added since Ver.5.0.0</span></small> |
|[Message](/package/extension4/progressbar/properties/message) | CRW | String |  |Message string for the window that pops up<br><small><span style="color:red">Added since Ver.5.0.0</span></small> |
|[PopupBgColor](/package/extension4/progressbar/properties/popupbgcolor) | CRW | integer |  | Background color of the window that pops up<br><small><span style="color:red">Added since Ver.5.0.0</span></small>|
|[PopupFgColor](/package/extension4/progressbar/properties/popupfgcolor) | CRW | integer |  |Text color of the message in the window that pops up<br><small><span style="color:red">Added since Ver.5.0.0</span></small> |
|[Position](/package/extension4/progressbar/properties/position) | CR | integer | $DTCENTER |Display position of the window to be displayed in a pop-up |
|[Step](/package/extension4/progressbar/properties/step) | CRW | integer | 1 | Maximum value of progress bar steps|
|[Title](/package/extension4/progressbar/properties/title) | CRW | String |  | The title of the pop-up window|
|[ToolTip](/package/extension4/progressbar/properties/tooltip) | CRW | String |  |Tool tip |
|[ToolTipDelayTime](/package/extension4/progressbar/properties/tooltipdelaytime) | CRW | integer | 0 |Tool tip display time <br><small><span style="color:red">Added since Ver.4.2.0</span></small> |
|[Value](/package/extension4/progressbar/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Object value <br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property