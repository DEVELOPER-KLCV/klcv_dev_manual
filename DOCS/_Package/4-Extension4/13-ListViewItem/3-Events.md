---
layout: default

grand_parent: 4. Extension4 Package
parent: ListViewItem Class

title: Events
nav_order: 3
permalink: /package/extension4/listviewitem/events

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following events are defined in the ListViewItem class.

|Name       | Description   |
|----------	|---------------|
|[Clicked](/package/extension4/listviewitem/events/clicked)|Occurs when clicking an item |
|[DoubleClicked](/package/extension4/listviewitem/events/doubleclicked)|Occurs when double-clicking an item|
|[RClicked](/package/extension4/listviewitem/events/rclicked)| Occurs when right-clicking on an item|
|[Touch](/package/extension4/listviewitem/events/touch)|Occurs when the item selection status changes |

### Precautions when referring to selection items<br>
In the handler of the event that occurred in the ListViewItem class, do not use the <a href="/package/extension4/listview/properties/value">Value</a> property of the parent object <a href="/package/extension4/listview">ListView</a> class to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the <a href="/package/system/event/properties/from">From</a> property (ListViewItem object) of the <a href="/package/system/event">Event</a> object passed as an argument of the event handler. For the selected state of the item, refer to the <a href="/package/extension4/listviewitem/properties/selected">Selected</a> property from the From property.

