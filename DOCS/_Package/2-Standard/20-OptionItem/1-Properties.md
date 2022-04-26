---
layout: default

grand_parent: 2. Standard Package
parent: OptionItem Class

title: Properties
nav_order: 1
permalink: /package/standard/optionitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the OptionItem class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[Selected](/package/standard/optionitem/properties/selected) | CRW | boolean | $FALSE  |             |
|[Title](/package/standard/optionitem/properties/title) | CRW | String<br>UString(※) |   |             |
|[ToolTip](/package/standard/optionitem/properties/tooltip) | CRW | String |   |             |
|[ToolTipDelayTime](/package/standard/optionitem/properties/tooltipdelaytime) | CRW | integer | 0  |             |
|[Value](/package/standard/optionitem/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |   |             |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
