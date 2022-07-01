---
layout: default

grand_parent: 4. Extension4 Package
parent: ListViewItem Class

title: Properties
nav_order: 1
permalink: /package/extension4/listviewitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ListViewItem class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[BgColor](/package/extension4/listviewitem/properties/bgcolor) | CRW | integer | $STD |Background color |
|[Bold](/package/extension4/listviewitem/properties/bold) | CRW | boolean | $FALSE |Bold line |
|[Checked](/package/extension4/listviewitem/properties/checked) | CRW | boolean | $FALSE |Check box selection |
|[FgColor](/package/extension4/listviewitem/properties/fgcolor) | CRW | integer | $STD |Font color |
|[Format](/package/extension4/listviewitem/properties/format) | CR | String |  |Formatting string |
|[Icon](/package/extension4/listviewitem/properties/icon) | CRW | integer | 0 |Image list icon index number |
|[Selected](/package/extension4/listviewitem/properties/selected) | CRW | boolean | $FALSE |Row selection |
|[Value](/package/extension4/listviewitem/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  | Item font|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property