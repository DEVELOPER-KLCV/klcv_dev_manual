---
layout: default

grand_parent: 2. Standard Package
parent: PulldownItem Class

title: Properties
nav_order: 1
permalink: /package/standard/pulldownitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the PulldownItem class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[Selected](/package/standard/pulldownitem/properties/selected) | CRW | boolean | $FALSE  | Item selection status            |
|[Title](/package/standard/pulldownitem/properties/title) | CRW | String<br>UString(※) |   |   Character string displayed in the options<br>(※)When ValueType is UString <br><br><small><span style="color:red">Added since Ver.5.0.3</span></small>           |
|[Value](/package/standard/pulldownitem/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date<br>UString |   |    Object Value <br><br><small><span style="color:green">Added UString since Ver.4.2.0             |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
