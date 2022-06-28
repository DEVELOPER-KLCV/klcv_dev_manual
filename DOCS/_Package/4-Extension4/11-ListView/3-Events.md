---
layout: default

grand_parent: 4. Extension4 Package
parent: ListView Class

title: Events
nav_order: 3
permalink: /package/extension4/listview/events

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following events are defined in the ListView class.

|Name       | Description   |
|----------	|---------------|
|[Clicked](/package/extension4/listview/events/clicked)| Occurs when the left mouse button is clicked|
|[DoubleClicked](/package/extension4/listview/events/doubleclicked)| Occurs when the left mouse button is double-clicked|
|[Dropped](/package/extension4/listview/events/dropped)| Occurs when dropped by drag and drop<br><small><span style="color:red">Added since Ver.4.1.0</span></small>|
|[RClicked](/package/extension4/listview/events/rclicked)|Occurs when the right mouse button is clicked |

※ When each item in ListView is clicked, the Clicked event of ListViewItem is generated. If you want to raise the Clicked event of the ListView, click anywhere other than the item.