---
layout: default

grand_parent: FlexView Class
parent: FlexCheckButton Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexcheckbutton/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexCheckButton class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[Active](/package/extension4/flexview/flexcheckbutton/properties/active) | CRW | boolean | $TRUE | Active state|
|[Border](/package/extension4/flexview/flexcheckbutton/properties/border) | CRW | boolean | $FALSE | Display frame|
|[BorderStyle](/package/extension4/flexview/flexcheckbutton/properties/borderstyle) | CRW | integer | $SUNKEN |Border style |
|[Selected](/package/extension4/flexview/flexcheckbutton/properties/selected) | CRW | boolean | $TRUE |Checked status |
|[Value](/package/extension4/flexview/flexcheckbutton/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | Cell default value <br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>|

Only for Mobile, Android version 

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[UseTapAndHold](/package/extension4/flexview/flexcheckbutton/properties/usetapandhold) | CRW | boolean | $FALSE |Whether to use tap and hold operation <br><small><span style="color:red">Added since AI Ver.1.0.0, Mobile Ver.3.0.0</span></small>| 

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: Default property