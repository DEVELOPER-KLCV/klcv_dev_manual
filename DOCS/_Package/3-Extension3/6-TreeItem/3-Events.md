---
layout: default

grand_parent: 3. Extension3 Package
parent: TreeItem Class

title: Events
nav_order: 3
permalink: /package/extension3/treeitem/events

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following events are defined in the TreeItem class.

|Name     | Description |
|---------|-------------|
|[Clicked](/package/extension3/treeitem/events/clicked) ||
|[DoubleClicked](/package/extension3/treeitem/events/doubleclicked) ||
|[Expand](/package/extension3/treeitem/events/expand) ||
|[Fold](/package/extension3/treeitem/events/fold) ||
|[GetFocus](/package/extension3/treeitem/events/getfocus) ||
|[LostFocus](/package/extension3/treeitem/events/lostfocus) ||
|[RClicked](/package/extension3/treeitem/events/rclicked) ||
|[Touch](/package/extension3/treeitem/events/touch) ||

<b>Precautions when referencing selection items</b>

Do not use the [Value](/package/extension3/treeview/properties/value) property of the parent object [TreeView](/package/extension3/treeview) class to refer to the selected item number in the handler of the event that occurred in the TreeItem class. (The selected item number may not be reflected.)

To refer to the selected item, use the [From](/package/system/event/properties/from) property (TreeItem object) of the Event object passed as an argument of the event handler.