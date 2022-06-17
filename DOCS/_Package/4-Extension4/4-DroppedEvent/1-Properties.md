---
layout: default

grand_parent: 4. Extension4 Package
parent: DroppedEvent Class

title: Properties
nav_order: 1
permalink: /package/extension4/droppedevent/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the DroppedEvent class.

|Name       | Access | Type   | Description |
|----------	|--------|--------|-------------|
|[AltKey](/package/extension4/droppedevent/properties/altkey) | CR | boolean |Pressing state of Alt key when dropped |
|[CtrlKey](/package/extension4/droppedevent/properties/ctrlkey) | CR | boolean | Pressing state of Ctrl key when dropped|
|[Data](/package/extension4/droppedevent/properties/data) | CR | Object |Dropped data |
|[LButton](/package/extension4/droppedevent/properties/lbutton) | CR | boolean | Pressing state of left mouse button when dropped|
|[MButton](/package/extension4/droppedevent/properties/mbutton) | CR | boolean | Pressing state of middle mouse button when dropped|
|[Mode](/package/extension4/droppedevent/properties/mode) | CR | integer |Whether drag and drop is in copy mode or move mode <br><small><span style="color:red">Added since Ver.5.0.0</span></small> |
|[RButton](/package/extension4/droppedevent/properties/rbutton) | CR | boolean | Pressing state of right mouse button when dropped|
|[ShiftKey](/package/extension4/droppedevent/properties/shiftkey) | CR | boolean | Pressing state of Shift key when dropped
|[Type](/package/extension4/droppedevent/properties/type) | CR | integer |Format of dropped data |
|[XPos](/package/extension4/droppedevent/properties/xpos) | CR | integer |Dropped X coordinate |
|[YPos](/package/extension4/droppedevent/properties/ypos) | CR | integer |Dropped Y coordinate |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable
