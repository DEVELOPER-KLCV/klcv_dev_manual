---
layout: default

grand_parent: FlexView Class
parent: FlexLabel Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexlabel/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexLabel class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[Border](/package/extension4/flexview/flexlabel/properties/border) | CRW | boolean | $FALSE |Display frame |
|[BorderStyle](/package/extension4/flexview/flexlabel/properties/borderstyle) | CRW | integer | $SUNKEN | Frame type |
|[Icon](/package/extension4/flexview/flexlabel/properties/icon) | CRW | integer | 0 | Initial value of icon number to be displayed in cell|
|[Value](/package/extension4/flexview/flexlabel/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  |Initial value of cell <br><small><span style="color:green">Added UStringsince Ver.4.2.0</span></small>|


Only for Mobile, Android version 

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[UseTapAndHold](/package/extension4/flexview/flexlabel/properties/usetapandhold) | CRW | boolean | $FALSE |Whether to use tap and hold operation<br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small> |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property