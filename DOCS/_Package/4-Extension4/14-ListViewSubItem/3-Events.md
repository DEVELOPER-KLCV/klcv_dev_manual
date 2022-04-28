---
layout: default

grand_parent: 4. Extension4 Package
parent: ListViewSubItem Class

title: Events
nav_order: 3
permalink: /package/extension4/listviewsubitem/events

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following events are defined in the ListViewSubItem class.

|Name       | Description     |
|----------	|-----------------|
|[Clicked](/package/extension4/listviewsubitem/events/clicked) | |
|[DoubleClicked](/package/extension4/listviewsubitem/events/doubleclicked) | |
|[RClicked](/package/extension4/listviewsubitem/events/rclicked) | |

<b>Precautions when referencing selection items</b>

Do not use the [Value]() property of the parent object [ListView]() class to refer to the selected item number in the handler of the event that occurred in the ListViewSubItem class. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the parent object ([ListViewItem]() object, which can be referenced by From. ^) of the [From]() property of the [Event]() object passed as an argument of the event handler.