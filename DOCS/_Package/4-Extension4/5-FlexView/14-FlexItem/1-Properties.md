---
layout: default

grand_parent: FlexView Class
parent: FlexItem Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexItem class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[Title](/package/extension4/flexview/flexitem/properties/title) | CRW | String<br>UString(※) | | Column title <br>(※) When ValueType is UString <br><small><span style="color:red">Added since Ver.5.0.3</span></small>|
|[TitleBgColor](/package/extension4/flexview/flexitem/properties/titlebgcolor) | CRW | integer |  $STD | Title background color<br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[TitleFgColor](/package/extension4/flexview/flexitem/properties/titlefgcolor) | CRW | integer | $STD |Title font color<br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[TitleHorzAlign](/package/extension4/flexview/flexitem/properties/titlehorzalign) | CR | integer | $STD | Title horizontal layout<br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[TitleMarker](/package/extension4/flexview/flexitem/properties/titlemarker) | CRW | integer | 0 |Specify the title marker <br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[TitleResize](/package/extension4/flexview/flexitem/properties/titleresize) | CRW | boolean | $FALSE |Column width changeability<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small> |
|[TitleRows](/package/extension4/flexview/flexitem/properties/titlerows) | CR | integer | 0 |Title occupancy <br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[TitleVertAlign](/package/extension4/flexview/flexitem/properties/titlevertalign) | CR | integer | $STD |Title vertical layout<br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[Width](/package/extension4/flexview/flexitem/properties/width) | CRW | integer | 100 |Column width |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable