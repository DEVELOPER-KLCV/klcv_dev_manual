---
layout: default

grand_parent: 4. Extension4 Package
parent: ComboBox Class

title: Properties
nav_order: 1
permalink: /package/extension4/combobox/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the ComboBox class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoTab](/package/extension4/combobox/properties/autotab) | CRW | boolean | $FALSE | Whether to automatically move the focus to the next object|
|[DropdownKey](/package/extension4/combobox/properties/dropdownkey) | CR | integer |  | Drop down key <br><small><span style="color:red">Added since Ver.5.0.0</span></small>|
|[DropdownWidth](/package/extension4/combobox/properties/dropdownwidth) | CR | integer |  | Dropdown width|
|[Editable](/package/extension4/combobox/properties/editable) | CRW | boolean | $TRUE | Whether to allow the user to enter any value|
|[InputMode](/package/extension4/combobox/properties/inputmode) | CR | integer |  | Specifying the character types that can be entered <br><small><span style="color:green">Specifiable values have been added since Ver.5.0.3</span></small>|
|[SelectionMode](/package/extension4/combobox/properties/selectionmode) | CR | integer | 0 | How to select from the options|
|[Value](/package/extension4/combobox/properties/value)* | CRW | String<br>UString |  | Value to be displayed in the text box<br><small><span style="color:green">UString have been added since Ver.5.0.3</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
