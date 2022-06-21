---
layout: default

grand_parent: FlexView Class
parent: FlexHeader Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexheader/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexHeader class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[Border](/package/extension4/flexview/flexheader/properties/border) | CRW | boolean | $FALSE |Display frame |
|[BorderStyle](/package/extension4/flexview/flexheader/properties/borderstyle) | CRW | integer | $SUNKEN |Border style |
|[HorizontalAlign](/package/extension4/flexview/flexheader/properties/horizontalalign) | CR | integer | $STD |Horizontal alignment |
|[Icon](/package/extension4/flexview/flexheader/properties/icon) | CRW | integer | 0 |Icon number <br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[Numbered](/package/extension4/flexview/flexheader/properties/numbered) | CRW | boolean | $FALSE | Display line number|
|[Value](/package/extension4/flexview/flexheader/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | Initial cell value<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|


Only for Mobile, Android version 

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[UseTapAndHold](/package/extension4/flexview/flexheader/properties/usetapandhold) | CRW | boolean | $FALSE |Whether to use tap and hold operation <br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property