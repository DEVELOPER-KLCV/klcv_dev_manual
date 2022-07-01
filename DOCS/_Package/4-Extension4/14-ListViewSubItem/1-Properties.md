---
layout: default

grand_parent: 4. Extension4 Package
parent: ListViewSubItem Class

title: Properties
nav_order: 1
permalink: /package/extension4/listviewsubitem/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ListViewSubItem class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[BgColor](/package/extension4/listviewsubitem/properties/bgcolor) | CRW | integer | $STD | Background color |
|[FgColor](/package/extension4/listviewsubitem/properties/fgcolor) | CRW | integer | $STD | Font color |
|[Format](/package/extension4/listviewsubitem/properties/format) | CR | String |  | Formatting string <br><small><span style="color:red">Formats that can be specified have been added since Ver.4.1.0</span></small>|
|[Value](/package/extension4/listviewsubitem/properties/value)* | CRW | String<br>Number<br>Fixed<br>Date |  | Item font|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property