---
layout: default

grand_parent: 2. Standard Package
parent: CheckBox Class

title: Properties
nav_order: 1
permalink: /package/standard/checkbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the CheckBox class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[BgColor](/package/standard/checkbox/properties/bgcolor) | CRW | integer | $STD | Background color |
|[Border](/package/standard/checkbox/properties/border) | CR | boolean | $FALSE | border display |
|[FgColor](/package/standard/checkbox/properties/fgcolor) | CRW | integer | $STD | Font color |
|[FontFace](/package/standard/checkbox/properties/fontface) | CR | integer | $STD | Font decoration attributes<br>**<small>There are limits in AI</small>**|
|[FontKind](/package/standard/checkbox/properties/fontkind) | CR | integer | $STD | Font type<br>**<small>Supported fonts have been added from Version2</small>**<br>**<small>Not supported in Mobile</small>**<br>**<small>There are limits in AI</small>**|
|[FontSize](/package/standard/checkbox/properties/fontsize) | CR | integer | 10 | Font size |
|[Scroll](/package/standard/checkbox/properties/scroll) | CR | integer | $AUTO | Scroll bar display control<br>**<small>There are limits in AI</small>**<br>**<small>There are no restrictions from Mobile Version 3.0.0</small>**  |
|[ToolTip](/package/standard/checkbox/properties/tooltip) | CRW | String |  | Tooltip<br>**<small>Not supported in Mobile, AI</small>**  |
|[ToolTipDelayTime](/package/standard/checkbox/properties/tooltipdelaytime) | CRW | integer | 0 | Tooltip display time<br>**<small>Added since Version 4.2.0</small>**<br>**<small>Not supported since Mobile, AI</small>**  |
|[Value](/package/standard/checkbox/properties/value)* | CRW | integer | | Selected position |


<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property