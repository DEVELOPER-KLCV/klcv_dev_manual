---
layout: default

grand_parent: 2. Standard Package
parent: CheckItem Class

title: Properties
nav_order: 1
permalink: /package/standard/checkitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the CheckItem class.

|Name       | Access | Type   | Initial Value |  Description |
|----------	|--------|--------|---------------|--------------|
|[Selected](/package/standard/checkitem/properties/selected) | CRW | boolean | $FALSE | Item selection status |
|[Title](/package/standard/checkitem/properties/title) | CRW | String<br>UString(※) | |The string displayed in the choices<br>(※) when ValueType is UString**<small>Added since Version 5.0.3</small>** |
|[ToolTip](/package/standard/checkitem/properties/ToolTip) | CRW | String |  | Item Tooltip<br>**<small>Added since Version 4.2.0</small>**<br>**<small>Not supported in Mobile, AI</small>** |
|[ToolTipDelayTime](/package/standard/checkitem/properties/ToolTipDelayTime) | CRW | integer | 0 | Tooltip display time<br>**<small>Added since Version 4.2.0</small>**<br>**<small>Not supported in Mobile, AI</small>** |
|[Value](/package/standard/checkitem/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |  | ItemObject value<br>**<small>UString added since Version 4.2.0</small>** |


<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property