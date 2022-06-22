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
|[Active](/package/extension4/flexview/flexlistbox/properties/active) | CRW | boolean |  $TRUE | Specify the activity|
|[AutoCursorMove](/package/extension4/flexview/flexlistbox/properties/autocursormove) | CR | boolean |  $FALSE |Cell cursor auto-movement <br><small><span style="color:red">Added since Ver.4.1.0</span></small> |
|[Border](/package/extension4/flexview/flexlistbox/properties/border) | CRW | boolean |  $FALSE |Frame display |
|[BorderStyle](/package/extension4/flexview/flexlistbox/properties/borderstyle) | CRW | integer |   | Border style|
|[DropdownKey](/package/extension4/flexview/flexlistbox/properties/dropdownkey) | CR | integer |   |Specify key to drop down <br><small><span style="color:red">Added since Ver.5.0.0, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small> |
|[KeySelect](/package/extension4/flexview/flexlistbox/properties/keyselect) | CRW | boolean | $FALSE  | Whether item selection by key input is possible<br><small><span style="color:red">Added since Ver.5.0.1, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small>|
|[ListData](/package/extension4/flexview/flexlistbox/properties/listdata) | CRW | String<br>UString(※) | | List options (※)When Valuetype is UString, <br><small><span style="color:red">added since Ver.5.0.3</span></small> |
|[Value](/package/extension4/flexview/flexlistbox/properties/value)* | CRW | String<br>UString | | Initial value of cell|

Only for Mobile version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[DropdownStyle](/package/extension4/flexview/flexlistbox/properties/dropdownstyle) | CR | integer |  $STD |How to display the selection list<br><small><span style="color:red">Added since Mobile Ver.4.5.0</span></small> |

Only for both Mobile and Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|----------|
|[UseTapAndHold](/package/extension4/flexview/flexlistbox/properties/usetapandhold) | CRW | boolean |  $FALSE |Whether to use tap and hold operation <br><small><span style="color:red">Added since Mobile Ver.3.0.0</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property