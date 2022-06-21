---
layout: default

grand_parent: FlexView Class
parent: FlexData Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexdata/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexData class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[BgColor](/package/extension4/flexview/flexdata/properties/bgcolor) | CRW | integer | $STD |Background color |
|[Data](/package/extension4/flexview/flexdata/properties/data) | CRW | String |  |General purpose data<br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[FgColor](/package/extension4/flexview/flexdata/properties/fgcolor) | CRW | integer | $STD | Font color|
|[Format](/package/extension4/flexview/flexdata/properties/format) | CR | String |  |Format string<br><small><span style="color:green">Supported fonts have been added since Ver.4.1.0</span></small> |
|[HorizontalAlign](/package/extension4/flexview/flexdata/properties/horizontalalign) | CR | integer | $STD |Horizontal layout |
|[ToolTip](/package/extension4/flexview/flexdata/properties/tooltip) | CRW | String |  | Tooltip<br><small><span style="color:red">Added since Ver.4.2.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Value](/package/extension4/flexview/flexdata/properties/value)* | CRW | ※ |  | Initial cell value|
|[VerticalAlign](/package/extension4/flexview/flexdata/properties/verticalalign) | CR | integer | $STD |Vertical layout |

※Depends on the ValueType of the inherited class

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property