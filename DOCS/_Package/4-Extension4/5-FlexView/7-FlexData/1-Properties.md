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
|[BgColor](/package/extension4/flexview/flexdata/properties/bgcolor) | CRW | integer | $STD | |
|[Data](/package/extension4/flexview/flexdata/properties/data) | CRW | String |  | |
|[FgColor](/package/extension4/flexview/flexdata/properties/fgcolor) | CRW | integer | $STD | |
|[Format](/package/extension4/flexview/flexdata/properties/format) | CR | String |  | |
|[HorizontalAlign](/package/extension4/flexview/flexdata/properties/horizontalalign) | CR | integer | $STD | |
|[ToolTip](/package/extension4/flexview/flexdata/properties/tooltip) | CRW | String |  | |
|[Value](/package/extension4/flexview/flexdata/properties/value)* | CRW | ※ |  | |
|[VerticalAlign](/package/extension4/flexview/flexdata/properties/verticalalign) | CR | integer | $STD | |

※Depends on the ValueType of the inherited class

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property