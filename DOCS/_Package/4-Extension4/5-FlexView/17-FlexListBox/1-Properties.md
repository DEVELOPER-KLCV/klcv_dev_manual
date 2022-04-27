---
layout: default

grand_parent: FlexView Class
parent: FlexListBox Class

title: Properties
nav_order: 1
permalink: /package/extension4/flexview/flexlistbox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the FlexListBox class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[Active](/package/extension4/flexview/flexlistbox/properties/active) | CRW | boolean |  $TRUE | |
|[AutoCursorMove](/package/extension4/flexview/flexlistbox/properties/autocursormove) | CR | boolean |  $FALSE | |
|[Border](/package/extension4/flexview/flexlistbox/properties/border) | CRW | boolean |  $FALSE | |
|[BorderStyle](/package/extension4/flexview/flexlistbox/properties/borderstyle) | CRW | integer |   | |
|[DropdownKey](/package/extension4/flexview/flexlistbox/properties/dropdownkey) | CR | integer |   | |
|[KeySelect](/package/extension4/flexview/flexlistbox/properties/keyselect) | CRW | boolean | $FALSE  | |
|[ListData](/package/extension4/flexview/flexlistbox/properties/listdata) | CRW | String<br>UString(※) | | |
|[Value](/package/extension4/flexview/flexlistbox/properties/value)* | CRW | String<br>UString | | |

Only for Mobile version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[DropdownStyle](/package/extension4/flexview/flexlistbox/properties/dropdownstyle) | CR | integer |  $STD | |

Only for both Mobile and Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[UseTapAndHold](/package/extension4/flexview/flexlistbox/properties/usetapandhold) | CRW | boolean |  $FALSE | |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property