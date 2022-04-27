---
layout: default

grand_parent: FlexView Class
parent: FlexCell Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexcell/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexCell class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[BgColor](/package/extension4/flexview/flexcell/properties/bgcolor) | CRW | integer | $STD | |
|[Data](/package/extension4/flexview/flexcell/properties/data) | CRW | String |  | |
|[FgColor](/package/extension4/flexview/flexcell/properties/fgcolor) | CRW | integer | $STD | |
|[ToolTip](/package/extension4/flexview/flexcell/properties/tooltip) | CRW | String |  | |
|[Value](/package/extension4/flexview/flexcell/properties/value)* | CRW | ※ |  | |

※Determined by the ValueType of the underlying FlexData inherited class.

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: Default property